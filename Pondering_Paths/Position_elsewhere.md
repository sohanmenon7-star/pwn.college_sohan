# Challenge 4 : Position elsewhere
In this challenge you are to change directories and then invoke a program

## My solve
**Flag:** `pwn.college{Ez56NEsktCUjrt0KDonwgUoPwHl.QX3QTN0wiM5kjNzEzW}`

As done in the previous challenge, `/challenge/run` to find the directory and then change and invoke the program
```
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /var/lib/apt/lists directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /var/lib/apt/lists
hacker@paths~position-elsewhere:/var/lib/apt/lists$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Ez56NEsktCUjrt0KDonwgUoPwHl.QX3QTN0wiM5kjNzEzW}
```

## What I learned 
Similar to the previous challenge, I learnt to change directories to the desired directory

## Incorrect tangents 
N/A

## References 
N/A
