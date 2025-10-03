# Challenge 2 : Killing Processes
The challenge asks you to kill a process using `kill` and then running the program with the flag

## My solve
**Flag:** `pwn.college{csjMDrGCgjtuPlhsLg5IgZRa_Ww.QXyQDO0wiM5kjNzEzW}`

- As explained in the cha;;enge, I simply used `ps aux` to find the /challenge/dont-run and then terminated the process using `kill` to obtain the flag
```
hacker@processes~killing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.1  0.0   1056   640 ?        Ss   04:08   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-works
root           7  0.0  0.0 231708  2560 ?        S    04:08   0:00 /run/dojo/bin/sleep 6h
root         135  0.0  0.0   5204  3520 ?        S    04:08   0:00 su -c /challenge/.launcher hacker
hacker       136  0.0  0.0 231576  3520 ?        Ss   04:08   0:00 /challenge/dont_run
hacker       137  0.0  0.0 231708  2560 ?        S    04:08   0:00 sleep 6h
hacker       139  0.0  0.0 231576  3520 pts/0    Ss   04:08   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-inte
hacker       145  0.0  0.0 231940  4160 pts/0    S    04:08   0:00 /run/dojo/bin/bash --login
hacker       155  0.0  0.0 233600  3840 pts/0    R+   04:09   0:00 ps aux
hacker@processes~killing-processes:~$ kill 136
hacker@processes~killing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   04:08   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-works
root           7  0.0  0.0 231708  2560 ?        S    04:08   0:00 /run/dojo/bin/sleep 6h
hacker       137  0.0  0.0 231708  2560 ?        S    04:08   0:00 sleep 6h
hacker       139  0.0  0.0 231576  3520 pts/0    Ss   04:08   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-inte
hacker       145  0.0  0.0 231940  4160 pts/0    S    04:08   0:00 /run/dojo/bin/bash --login
hacker       156  0.0  0.0 233600  3840 pts/0    R+   04:10   0:00 ps aux
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{csjMDrGCgjtuPlhsLg5IgZRa_Ww.QXyQDO0wiM5kjNzEzW}
```

## What I learned 
I learned about killing processes using the `kill` command. The `kill` command takes the PID of a process as its argument to terminate it

## Incorrect tangents 
N/A

## References 
N/A
