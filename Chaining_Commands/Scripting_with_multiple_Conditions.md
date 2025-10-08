# Challenge 11 : Scripting with Multiple Conditions
This chllenge adds to the previous challenge, by adding multiple conditions using `elif` in the shell script

## My solve
**Flag:** `pwn.college{85zHGnN-FSkVn1yzPmeDiEGuv4O.0FOzMDOxwiM5kjNzEzW}`

- Firstly I touched solve.sh and used `nano` to write the if conditional statements
- I additionally wrote `elif` parts
- I then ran the program to obtain the result
```
hacker@chaining~scripting-with-multiple-conditions:~$ touch solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ nano solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ cat solve.sh
#!/bin/bash

if [ "$1" == "pwn" ]
then
    echo "college"
elif [ "$1" == "hack" ]
then
    echo "the planet"
elif [ "$1" == "learn" ]
then
    echo linux
else
    echo nope
fi
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Test failed for input 'foo'
Expected: 'unknown'
Got: 'nope'
hacker@chaining~scripting-with-multiple-conditions:~$ nano solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{85zHGnN-FSkVn1yzPmeDiEGuv4O.0FOzMDOxwiM5kjNzEzW}
```

## What I learned 
I learned you can have multiple conditions in the shell script using `elif`

## Incorrect tangents 
Syntax Errors

## References 
N/A
