# Challenge 7 : Reading Inputs
This challenge asks you to input the values of a variable in the shell by providing it with stdin using `read`

## My solve
**Flag:** `pwn.college{8VJ7O-qRUiCUwAzajjhB5TMeLbN.QX4cTN0wiM5kjNzEzW}`

As explained in the challenge I used `read` with argument PWN vairable to accept input from the user and setting the value as COLLEGE. This gave me the flag
```
hacker@variables~reading-input:~$ read PWN
COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{8VJ7O-qRUiCUwAzajjhB5TMeLbN.QX4cTN0wiM5kjNzEzW}
```

## What I learned 
- I learnt that `read` can be used to accept input from the user and assign it to a variable
- Also, `read` can be upgraded by adding `-p` to it to specify a prompt

## Incorrect tangents 
N/A

## References 
N/A
