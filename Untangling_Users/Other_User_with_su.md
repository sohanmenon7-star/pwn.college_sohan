# Challenge 2 : Other users with su
The challenge simply requires you to use `su` in order to become user zardus and then running a program to obtain the file

## My solve
**Flag:** `pwn.college{Q36-RbXvBaV_513s4Ert2Q_P2cI.QX2UDN1wiM5kjNzEzW}`

- As asked in teh challenge, I used `su` command with zardus as the arguemnt since that is the username, to switch into zardus user
- After which I simply ran /challenge/run as told in the challenge, to obtain the flag
```
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{Q36-RbXvBaV_513s4Ert2Q_P2cI.QX2UDN1wiM5kjNzEzW}
```

## What I learned 
This challenge taught me about how you can specify the user you want to switch to by using `su` and giving the user name as the argument, meaning `su` is not only for changing user to `root`

## Incorrect tangents 
N/A

## References 
N/A
