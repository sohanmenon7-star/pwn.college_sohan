# Challenge 3 : Position thy self
In this challenge you are to change directories and then invoke a program

## My solve
**Flag:** `pwn.college{kMRBNYtFhll-LaGI35r5OmNJDCG.QX2QTN0wiM5kjNzEzW}`

- First input `/challenge/run` to find the directory to invoke the program from
- Once found, use `cd` to change directory and then invoke the program
```
hacker@paths~position-thy-self:/$ /challenge/run
Incorrect...
You are not currently in the /var/lib/apt/lists directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:/$ cd /var/lib/apt/lists
hacker@paths~position-thy-self:/var/lib/apt/lists$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{kMRBNYtFhll-LaGI35r5OmNJDCG.QX2QTN0wiM5kjNzEzW}
```

## What I learned 
I learnt to change directories to specified one and also to see the list of all directories

## Incorrect tangents 
N/A

## References 
N/A
