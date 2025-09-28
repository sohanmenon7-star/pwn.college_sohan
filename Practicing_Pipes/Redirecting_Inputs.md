# Challenge 5 : Redirecting Inputs
This question teaches you about redirecting inputs into a program using `<` from a file containing an output

## My solve
**Flag:** `pwn.college{gtQmKk9lJrJ2NF634-6z4WwSXY4.QXwcTN0wiM5kjNzEzW}` 

As told in the challenge, I started by redirecting an output of COLLEGE using `echo` to a file PWN
I then redirected this output to the program as input using `<` to obtain the flag
```
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{gtQmKk9lJrJ2NF634-6z4WwSXY4.QXwcTN0wiM5kjNzEzW}
```

## What I learned 
I leanrt about using `<` to redirect output from a file as input into a program

## Incorrect tangents 
N/A

## References 
N/A
