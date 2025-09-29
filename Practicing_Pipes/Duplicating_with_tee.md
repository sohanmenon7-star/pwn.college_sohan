# Challenge 10 : Dpulicating Piped output with tee
This challenge wants you to intercept the stdout and find out about what the program wants from you

## My solve
**Flag:** `pwn.college{UkGWkYKZml8GjdvUfloHaB9elFo.QXxITO0wiM5kjNzEzW}`

- As explained in the challenge, I intercepted the output of `/challenge/pwn` to a file 'intercept' using `tee` command to find out more about what pwn program wants
- After `cat`ing the intercept output to find out about what pwn wants I put the argument of the program and piped the stdout into `/challenge/college` as asked in the question
```
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee intercept | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat intercept
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "UkGWkYKZ"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret UkGWkYKZ | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{UkGWkYKZml8GjdvUfloHaB9elFo.QXxITO0wiM5kjNzEzW}
```

## What I learned 
- I learnt about the `tee` command which duplicates the data given flowing through the pipe operator
- I leared to use it to intercept output of a program to pull more information about the program

## Incorrect tangents 
N/A

## References 
N/A
