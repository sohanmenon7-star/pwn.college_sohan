# Challenge 2 : Programs and Absolute paths
The challenge requires you to invoke a program that is inside a different directory

## My solve
**Flag:** `pwn.college{QC9zY9u1kmFLsEa5_akW_LGgxrW.QX1QTN0wiM5kjNzEzW}`

As given in the challenge the program was told to be in the 'challenge' directory, thus by providing the absolute path of the program through the directory `/challenge/run` , this challenge was solved
```
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{QC9zY9u1kmFLsEa5_akW_LGgxrW.QX1QTN0wiM5kjNzEzW}
```

## What I learned 
Invoking a program within a specific directory by putting its absolute path

## Incorrect tangents 
N/A

## References 
N/A
