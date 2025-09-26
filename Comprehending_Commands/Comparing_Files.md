# Challenge 5 : Comparing Files
This challenge provides you with two large files and need to use the `diff` command to compare the files and find the flag

## My solve
**Flag:** `pwn.college{cRDY9LFYFKHFTYnlJ_WQj2_rysJ.01MwMDOxwiM5kjNzEzW}`

The challenge gave you the absolute paths of the files, So putting those as the arguments of the command to find the flag
```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
36a37
> pwn.college{cRDY9LFYFKHFTYnlJ_WQj2_rysJ.01MwMDOxwiM5kjNzEzW}
```

## What I learned 
I learnt that when needing to compare large files, using the `diff` command can help save a lot time and effort

## Incorrect tangents 
N/A

## References 
N/A
