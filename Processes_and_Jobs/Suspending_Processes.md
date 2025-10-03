# Challenge 5 : Suspending Processes
To obtain the flag in this challenge, You have to run a program, suspend it and run it again, only then will you obtain the flag

## My solve
**Flag:** `pwn.college{IGfevXoa170Xd2bsEtEtjlYn7ug.QX1QDO0wiM5kjNzEzW}`

- As explained in the challenge, I first used `ps aux` to find the decoy flag process
- Then I killed it using `kill` after which I ran /challenge/run to write the flag into the named pipe
- To obtain the flag, I simply `cat` the named pipe 
```
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         140     130  0 04:43 pts/0    00:00:00 bash /challenge/run
root         142     140  0 04:43 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         140     130  0 04:43 pts/0    00:00:00 bash /challenge/run
root         147     130  0 04:43 pts/0    00:00:00 bash /challenge/run
root         149     147  0 04:43 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{IGfevXoa170Xd2bsEtEtjlYn7ug.QX1QDO0wiM5kjNzEzW}
```

## What I learned 
I learned there is a less drastic way of getting the terminal back, that being `Ctrl-Z` which suspends the ongoig process, meaning it still runs just in the background

## Incorrect tangents 
N/A

## References 
N/A

