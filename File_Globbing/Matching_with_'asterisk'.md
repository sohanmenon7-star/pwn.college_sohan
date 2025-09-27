# Challenge 1 : Matching with *
The challenge wants you to use the glob `*` to change directory in less than 4 characters

## My solve
**Flag:** `pwn.college{kGQCRLDea3gmTYwb1Cve0_dmN35.QX0ETO0wiM5kjNzEzW}`

In the explaination of `*`, I found that you can put the start of the file name and follow it with a `*` to glob the file.
Using this, I inputted `cd /ch*` to change directories with an argument less than 4 characters
```
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{0EUF7XkLYuxUth9dqTOuuYZlezG.QXxIDO0wiM5kjNzEzW}
```

## What I learned 
This question taught me about the glob `*` and how it behaves as a wildcard, searching for patterns in names to complete the path

## Incorrect tangents 
N/A

## References 
N/A
