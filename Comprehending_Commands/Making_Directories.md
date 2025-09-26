# Challenge 12 : Making Directories
So far we have only learnt how to create files, this challenge will teach you how to make directory

## My solve
**Flag:** `pwn.college{QR6SetY55aw7bWxpZzrzvNWYSHS.QXxMDO0wiM5kjNzEzW}`

Using the `mkdir` command to create a directory in the given absolute path, to make a directory and change the current working directory to the newly created directory and invoking the program
```
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{QR6SetY55aw7bWxpZzrzvNWYSHS.QXxMDO0wiM5kjNzEzW}
```

## What I learned 
I learnt how to use the `mkdir` command to create a directory

## Incorrect tangents
N/A

## References
N/A
