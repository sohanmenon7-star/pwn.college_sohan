# Challenge 5 : Position yet elsewhere
In this challenge you are to change directories and then invoke a program

## My solve
**Flag:** `pwn.college{s_NyCECdoIH__YFhnCs-N8-lscF.QX4QTN0wiM5kjNzEzW}`

As done in the previous challenge, `/challenge/run` to find the directory, change directories and invoke the program

```
hacker@paths~position-elsewhere:~$ /challenge/run
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/build-essential directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /usr/share/build-essential
hacker@paths~position-yet-elsewhere:/usr/share/build-essential$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{s_NyCECdoIH__YFhnCs-N8-lscF.QX4QTN0wiM5kjNzEzW}
```

## What I learned 
Practicing changing directories to fully grasp the conept

## Incorrect tangents 
N/A

## References 
N/A
