# Challenge 8 : Scripting with Arguemnts
This challenge wants you to take two arguments and reverse the order in which they were entered then run a program to obtain the flag

## My solve
**Flag:** `pwn.college{42QGL8puCyz9H6mvvkvJOFRj7ed.0VNzMDOxwiM5kjNzEzW}`

- I touched a file solve.sh and wrote `echo $2 $1` in it which takes second argument and prints that first
- This got the flag
```
hacker@chaining~scripting-with-arguments:~$ touch solve.sh
hacker@chaining~scripting-with-arguments:~$ nano solve.sh
hacker@chaining~scripting-with-arguments:~$ cat solve.sh
#!/bin/bash

echo $2 $1
hacker@chaining~scripting-with-arguments:~$ /challenge/run
Correct! Your script properly reversed the arguments.
Here's your flag:
pwn.college{42QGL8puCyz9H6mvvkvJOFRj7ed.0VNzMDOxwiM5kjNzEzW}
```

## What I learned 
This challenge taught me that the use of arguments in script is possible by using special variable `$1` which indicates the first argument

## Incorrect tangents 
N/A

## References 
N/A
