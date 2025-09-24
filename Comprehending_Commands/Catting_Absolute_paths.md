# Challenge 2 : Catting Absolute paths
This challenge wants you to use an absolute path as the argument for `cat`

## My solve
**Flag:** `pwn.college{wj7LAP-H9VF4cNvkMHjZ8MSEbsj.QX5ETO0wiM5kjNzEzW}`

The absolute path was given in the challenge, putting that as the argument for `cat` gave me the flag
```
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{wj7LAP-H9VF4cNvkMHjZ8MSEbsj.QX5ETO0wiM5kjNzEzW}
```

## What I learned
I learnt that the `cat` command accepts absolute paths as an argument and will directly read the file without the need to change directories

## Incorrect tangents 
N/A.

## References 
N/A
