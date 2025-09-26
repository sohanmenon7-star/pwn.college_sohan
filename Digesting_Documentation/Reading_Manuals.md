# Challenge 3 : Reading Manuals
This challenge asks you to read the manual of a command using the `man` command to get information on how to obtain the flag

## My solve
**Flag:** `pwn.college{AHngfMHu4i2MnD8SJn7IYsVSKhP.QX0EDO0wiM5kjNzEzW}`

As told in the challenge, I used the `man` command and put the argument of challenge to open the manual about the command.
In the manual, it was stated in the description that I had to input a specific argument to obtain the flag
```
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --ngfuin NUM 428
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ /challenge/challenge --ngfuin 428
Correct usage! Your flag: pwn.college{AHngfMHu4i2MnD8SJn7IYsVSKhP.QX0EDO0wiM5kjNzEzW}
```

## What I learned 
I learned how to use the `man` command to obtain information about a command and using it solve questions and understand a certain command better

## Incorrect tangents 
I misinterpreted the desription provided by the manual

## References 
N/A
