# Challenge 6 : Implicit relative paths(from '/')
The challenge wants you to use relative paths to invoke a program

## My solve
**Flag:** `pwn.college{kj5pgqpi_YTltDRHIhc4jJ_HM6B.QX5QTN0wiM5kjNzEzW}`

- Firstly, as instructed in the challenge, change the directory to `/`
- Then input the relative path to invoke the program(No `/` at the start of the command)
```
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kj5pgqpi_YTltDRHIhc4jJ_HM6B.QX5QTN0wiM5kjNzEzW}
```

## What I learned 
I learnt about relative paths and how it depends on the current working directory `cwd` and most importantly does not begin with `/` 

## Incorrect tangents 
N/A

## References 
N/A
