# Challenge 11 : Process Substitution for Input
This challenge asks you to use the `diff` command to find the real flag between two program which will output multiple decoy flags

## My solve
**Flag:** `pwn.college{MXu90Yy9YnCRqM3IvSYmllNFKkc.0lNwMDOxwiM5kjNzEzW}`

As instructed, I simple used the `<()` command to feed output of the programs to the `diff` command as input
This found the difference in the lines which was the flag
```
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
82a83
> pwn.college{MXu90Yy9YnCRqM3IvSYmllNFKkc.0lNwMDOxwiM5kjNzEzW}
```

## What I learned 
- I learned about the `<()` command and how it is used to feed output as input
- This is done bycreating a temporary file of the output of the command and using that file as the argument to the command you are feeding the output to 

## Incorrect tangents 
N/A

## References 
N/A
