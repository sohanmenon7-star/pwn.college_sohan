# Challenge 4 : Matching paths with []
The challenge wants you to use the glob `[]` in an absolute path to cobtain the flag using the glob

## My solve
**Flag:** `pwn.college{8wQKuzsICR8XoWiCPpUsiysYy9Y.QX0IDO0wiM5kjNzEzW}`

As told, I ran the program with the absolute path `/challenge/files/file_[absh]` as argument to find the flag
```
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[absh]
You got it! Here is your flag!
pwn.college{8wQKuzsICR8XoWiCPpUsiysYy9Y.QX0IDO0wiM5kjNzEzW}
```

## What I learned 
I learnt that `[]` can be used in absolute paths to call multiple absolute paths with a singular argument

## Incorrect tangents 
N/A

## References 
N/A
