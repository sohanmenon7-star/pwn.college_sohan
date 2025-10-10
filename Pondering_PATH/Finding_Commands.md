# Challenge 3 : Finding Commands
In this challenge, the command `win` and the flag are in the same directory, you need to find the directory and then read the flag

## My solve
**Flag:** `pwn.college{kolWsvHSNjkT5Fm94pXmsZ0ZEZT.01NzEzNxwiM5kjNzEzW}`

- In the challenge it was told that `win` command and flag are in the same directory, thus I simply used `which` to find the location of `win` in $PATH 
- Then I simply used the path to find the flag and `cat` it
```
hacker@path~finding-commands:~$ which win
/challenge/paths/27043/win
hacker@path~finding-commands:~$ cat /challenge/paths/27043/flag
pwn.college{kolWsvHSNjkT5Fm94pXmsZ0ZEZT.01NzEzNxwiM5kjNzEzW}
```

## What I learned 
I learned about the `which` command which can be used to find out the path of a command stored in $PATH by passing the name of the command as the argument 

## Incorrect tangents 
N/A

## References 
N/A
