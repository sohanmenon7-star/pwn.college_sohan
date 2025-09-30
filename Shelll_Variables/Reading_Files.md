# Challenge 8 : Reading Files
This challenge is about using `<` to directly give stdin into the `read` command, assigning the value to the variable

## My solve
**Flag:** `pwn.college{0YDBInl1TTEdTYE0gqj2iOb1XXi.QXwIDO0wiM5kjNzEzW}`

As told in the challenge, I used `<` to redirect the stdout of /challenge/run into `read` and stdin and thus assigned the value of PWN, giving me the flag
```
hacker@variables~reading-files:~$ read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{0YDBInl1TTEdTYE0gqj2iOb1XXi.QXwIDO0wiM5kjNzEzW}
```

## What I learned 
I learnt how you can store output of files and read them very easil using the `read` command with `<` to directly give the file as stdin to it and set the value of the variable

## Incorrect tangents 
N/A

## References 
N/A
