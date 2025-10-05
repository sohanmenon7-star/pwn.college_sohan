# Challenge 4 : Using sudo
Challenge 4 is about using the new and improved `sudo` command to access `root` and obtain the flag buried in it

## My solve
**Flag:** `pwn.college{0pSCQ9o0wcYmM2mjzjdKWGWAmWk.QX4UDN1wiM5kjNzEzW}`

- As told in the challenge, I simply used `sudo` to gain access to root and ran the command `cat /flag` right after it to obtain the flag
```
hacker@users~using-sudo:~$ sudo cat /flag
pwn.college{0pSCQ9o0wcYmM2mjzjdKWGWAmWk.QX4UDN1wiM5kjNzEzW}
```

## What I learned 
- This challenge taught me about `sudo` which stands for 'substitute user, do'. What this means is that unlike `su` in which you need to provide a password and then it will change its shell for you to run commands in root, you simply use `sudo` which defaults to root and run a command without the hassle of inputing a password
- You need access to root before hand to use `sudo` 

## Incorrect tangents 
N/A

## References 
N/A
