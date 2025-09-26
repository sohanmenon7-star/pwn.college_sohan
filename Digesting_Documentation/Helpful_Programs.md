# Challenge 6 : Helpful Program
This challenge wants you to use `--help` instead of `man` to find out information about a given program

## My solve
**Flag:** `pwn.college{QAABEdDZLmTHWyBo2410zGMum8X.QX3IDO0wiM5kjNzEzW}`

As instructed in the argument, I simply put `--help` as the argument to the program.
This gave me the optional arguments that can be used with the program, in which I first had to use the `-p` argument to obtain the numcode which I had to put as the argument for the `-g` argument to find the flag
```
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 241
hacker@man~helpful-programs:~$ /challenge/challenge -g 241
Correct usage! Your flag: pwn.college{QAABEdDZLmTHWyBo2410zGMum8X.QX3IDO0wiM5kjNzEzW}
```

## What I learned 
This problem taught me about the `--help` arguemnt which can be used in stead of `man` in ase its not present

## Incorrect tangents 
N/A

## References 
N/A
