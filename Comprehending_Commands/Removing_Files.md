# Challenge 8 : Removing Files
What this challenge wants you to do is, use the `rm` command to delete a file

## My solve
**Flag:** `pwn.college{ojhlRm9pohjvDdwR3kw6VHwVqVX.QX2kDM1wiM5kjNzEzW}`

As told in the challenge, I first created the file using `touch` and then remove the file using `rm` command. Then obtain the flag using program to find the flag
```
hacker@commands~removing-files:~$ touch delete_me
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{ojhlRm9pohjvDdwR3kw6VHwVqVX.QX2kDM1wiM5kjNzEzW}
```

## What I learned 
I learnt how to remove unwanted files using the `rm` command by giving the file in the argument

## Incorrect tangents 
N/A

## References 
N/A
