# Challenge 4 : Redirecting errors
This challenge asks you to redirect multipple file descriptors at once by redirecting outputs to one file and errors to another

## My solve
**Flag:** `pwn.college{0ifqAwYEAF1-q6Jb1Ygj_DY6B3k.QX3YTN0wiM5kjNzEzW}` 

As instructed in the challenge, I redirected the output to myflag file and errors to instructions flag, thus nothing was told in the terminal after inputting the redirection
```
hacker@piping~redirecting-errors:~$ /challenge/run 1>myflag 2>instructions
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{0ifqAwYEAF1-q6Jb1Ygj_DY6B3k.QX3YTN0wiM5kjNzEzW}
```

## What I learned 
- I learned you can redirect multiple descriptors to seperate files at the same time
- Also I learnt about file descriptor number and how to use them to redirect stdin, stdout, stderr to seperate files by putting their respctive number in front of `>`

## Incorrect tangents 
N/A

## References 
N/A
