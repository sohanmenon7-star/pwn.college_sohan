# Challenge 9 : Scripting with Conditionals
This challenge requires you to use `if` to script a condition such that it should give an output based on a certain input by the user

## My solve
**Flag:** `pwn.college{UrsKL51F_3A2m_rDvz6oJQCxVkP.0lNzMDOxwiM5kjNzEzW}`

- Firstly I touched solve.sh and used `nano` to write the if conditional statements
- I then ran the program to obtain the result
```
hacker@chaining~scripting-with-conditionals:~$ touch solve.sh
hacker@chaining~scripting-with-conditionals:~$ nano solve.sh
hacker@chaining~scripting-with-conditionals:~$ cat solve.sh
#!/bin/bash

if[ $1 == "pwn"]
then
    echo college
fi
hacker@chaining~scripting-with-conditionals:~$ bash solve.sh pwn
solve.sh: line 3: if[ pwn == pwn]: command not found
solve.sh: line 4: syntax error near unexpected token `then'
solve.sh: line 4: `then'
hacker@chaining~scripting-with-conditionals:~$ nano solve.sh
hacker@chaining~scripting-with-conditionals:~$ bash solve.sh pwn
college
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{UrsKL51F_3A2m_rDvz6oJQCxVkP.0lNzMDOxwiM5kjNzEzW}
```

## What I learned 
- I learnt you can use conditional scripts in the shell script to get a value only for a certain desired value entered
- `if []` for the condition, `then` for the statment if the condition is true, `fi` to terminate the if condition

## Incorrect tangents 
Syntax Errors

## References 
N/A
