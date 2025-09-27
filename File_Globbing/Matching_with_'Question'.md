# Challenge 2 : Matching with ?
The challenge wants you to use the glob `?` to change directory and using the glob

## My solve
**Flag:** `pwn.college{MAJvE6dm_2Q0ICn4wLOcf4GalaJ.QXyIDO0wiM5kjNzEzW}`

As instructed in the challenge, I simple changes `c` and `l` with `?` to change directories and obtain the answer
```
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /?ha??enge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{MAJvE6dm_2Q0ICn4wLOcf4GalaJ.QXyIDO0wiM5kjNzEzW}
```

## What I learned 
This question taught me about the glob `?` and how it behaves as a single character wildcard, searching for patterns in names to complete the path

## Incorrect tangents 
N/A

## References 
N/A
