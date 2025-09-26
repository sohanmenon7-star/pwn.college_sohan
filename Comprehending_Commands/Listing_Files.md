# Challenge 6 : Listing files
This challenge requires you to list all the files and directories in a specified directory

## My solve
**Flag:** `pwn.college{wKYvC7g-ySTLFnXKNqDCYurfeqs.QX4IDO0wiM5kjNzEzW}`

As asked in the challenge, using `ls` command and the absolute path of the directory as the argument to find the program containing the flag
```
hacker@commands~listing-files:~$ ls /challenge
8277-renamed-run-20347  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/8277-renamed-run-20347
Yahaha, you found me! Here is your flag:
pwn.college{wKYvC7g-ySTLFnXKNqDCYurfeqs.QX4IDO0wiM5kjNzEzW}
```

## What I learned 
This challenge taught me how to use the `ls` command to list the files and directories within a directory to find a desired file/directory

## Incorrect tangents 
N/A

## References 
N/A
