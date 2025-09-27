# Challenge 7 : Exclusionary Globbing
This question is about the `[]` glob which can be changed by adding `!` at the start to exclude files starting with a certain character

## My solve
**Flag:** `pwn.college{IIYvrI4ny7GT2O_mr3pNEIcIsUE.QX2IDO0wiM5kjNzEzW}`

As told in the challenge description, I used the `[!pwn]*` arguemnt to the program to exclude files starting with 'p', 'w' and 'n'
```
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{IIYvrI4ny7GT2O_mr3pNEIcIsUE.QX2IDO0wiM5kjNzEzW}
```

## What I learned 
I learned about excluding unwanted files by using `[!]` argument to print many files as this is easier than mentioning the first character of all files

## Incorrect tangents 
N/A

## References 
N/A
