# Challenge 9 : Home Sweet Home
This challenge requires you to run the command `/challenge/run` with an argument. The argument will be the directory in which the file will be written. Additionally, the argument cannot be greater than 3 characters
## My solve
**Flag:** `pwn.college{MmSmmuONpyR2TRS8Nq_RgvKUt9d.QXzMDO0wiM5kjNzEzW}`

As told in the challenge, I started by running `/challenge/run` and in the argument `~/~` which is expanded to `/home/hacker/~`
Thus, the file was written within the home directory. Finally, to read the file I ran the `cat` command.
```
hacker@paths~home-sweet-home:~$ /challenge/run ~/~
Writing the file to /home/hacker/~!
... and reading it back to you:
pwn.college{MmSmmuONpyR2TRS8Nq_RgvKUt9d.QXzMDO0wiM5kjNzEzW}
hacker@paths~home-sweet-home:~$ ~/~
bash: /home/hacker/~: Permission denied
hacker@paths~home-sweet-home:~$ cat ~/~
pwn.college{MmSmmuONpyR2TRS8Nq_RgvKUt9d.QXzMDO0wiM5kjNzEzW}
```

## What I learned 
I learnt about the home directory and its shorthand `~` and the use case of it. Typically the `~` is set to the home directory since it is used most often.

## Incorrect tangents 
- In the challenge, it was written the directory in which the file will written is 3 characters or less, which means you had to use `~`, which was missed in the first attempt
- Once the file was written, I did not know how to read the file as that was told in later modules

## References 
N/A
