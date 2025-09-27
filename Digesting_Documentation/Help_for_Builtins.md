# Challenge 7 : Help for builtins
This challenge wants you to use the `help` command to first search for the builtin and then use it to obtain the flag

## My solve
**Flag:** `pwn.college{kGQCRLDea3gmTYwb1Cve0_dmN35.QX0ETO0wiM5kjNzEzW}`

As stated in the challenge, I used the `help` command with argument builtin `challenge` to learn about it.
Using this information I obtained the argument to `challenge` and found the flag
```
hacker@man~help-for-builtins:~$ help 
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "kGQCRLDe".
hacker@man~help-for-builtins:~$ challenge --secret kGQCRLDe
Correct! Here is your flag!
pwn.college{kGQCRLDea3gmTYwb1Cve0_dmN35.QX0ETO0wiM5kjNzEzW}
```

## What I learned 
This problem taught me about builtins, how to use them and learn about them with `help` command

## Incorrect tangents 
N/A

## References 
N/A
