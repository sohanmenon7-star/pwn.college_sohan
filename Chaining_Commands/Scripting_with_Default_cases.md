# Challenge 10 : Scripting with Default cases
This chllenge adds to the previous challenge, If the condition fails, print an appropriate default message

## My solve
**Flag:** `pwn.college{EKTAj7ZFbQyestntX-z90r_vDqr.01NzMDOxwiM5kjNzEzW}`

- Firstly I touched solve.sh and used `nano` to write the if conditional statements
- I additionally wrote `else` part, `echo nope`
- I then ran the program to obtain the result
```
hacker@chaining~scripting-with-default-cases:~$ touch solve.sh
hacker@chaining~scripting-with-default-cases:~$ nano solve.sh
hacker@chaining~scripting-with-default-cases:~$ cat solve.sh
#!/bin/bash

if [ "$1" == "pwn" ]
then
    echo "college"
else
    echo nope
fi
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{EKTAj7ZFbQyestntX-z90r_vDqr.01NzMDOxwiM5kjNzEzW}
```

## What I learned 
- I learnt about default statements in conditional scripts, which can be written using `else`
- `else` does not have a condition

## Incorrect tangents 
Syntax Errors

## References 
N/A
