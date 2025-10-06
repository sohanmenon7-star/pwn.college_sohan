# Challenge 1 : Changing File ownership
This challenge requires you to change ownership of the flag file using the `chown` command to hacker from root so you can read it

## My solve
**Flag:** `pwn.college{wgww6gh92q_ZNpE_5kNr3Ux_KJI.QXxEjN0wiM5kjNzEzW}`

As instructed, I simply used `chown` gave hacker and /flag as the arguments to change the owner and then `cat` the flag
```
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{wgww6gh92q_ZNpE_5kNr3Ux_KJI.QXxEjN0wiM5kjNzEzW}
```

## What I learned 
- I learnt how to use `ls -l` to read the information provided at a higher level getting to know the user that owns the file and the group that owns the flag
- I learned how to use that `chown` command to change owner to specified owner(Usually this can only be done if you are the root user)

## Incorrect tangents 
N/A

## References 
N/A
