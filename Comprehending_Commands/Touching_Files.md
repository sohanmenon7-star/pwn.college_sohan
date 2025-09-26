# Challenge 7 : Touching/Creating Files
The challenge asks you to create a new file in a specified directory using the `touch` command

## My solve
**Flag:** `pwn.college{06vHaXZOa2TY2aah6ygKhkdpfsK.QXwMDO0wiM5kjNzEzW}`

As instructed in the challenge, I used the `touch` command to create two files with the specified absolute paths as the argument and after which I ran the command `/challenge/run` as asked in the challenge
```
hacker@commands~touching-files:~$ touch /tmp/pwn
hacker@commands~touching-files:~$ ouch /tmp/college
bash: ouch: command not found
hacker@commands~touching-files:~$ touch /tmp/college
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{06vHaXZOa2TY2aah6ygKhkdpfsK.QXwMDO0wiM5kjNzEzW}
```

## What I learned 
I learnt how to use the `touch` command to create files in the specified locations by giving the paths as arguments or in the home directory by not putting an argument

## Incorrect tangents 
N/A

## References 
N/A
