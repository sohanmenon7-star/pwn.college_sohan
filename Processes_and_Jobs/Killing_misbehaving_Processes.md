# Challenge 4 : Killing Misbehaving Processes
This challenge asks you to kill a processes which creates decoy in a named pipe and then run the program to obtain the flag

## My solve
**Flag:** `pwn.college{IaZ_E_g5cDShzYAa3qXgwsFVWNY.0FNzMDOxwiM5kjNzEzW}`

- As explained in the challenge, I first used `ps aux` to find the decoy flag process
- Then I killed it using `kill` after which I ran /challenge/run to write the flag into the named pipe
- To obtain the flag, I simply `cat` the named pipe 
```
hacker@processes~killing-misbehaving-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.5  0.0   1056   640 ?        Ss   04:31   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-works
root           7  0.4  0.0 231708  2560 ?        S    04:31   0:00 /run/dojo/bin/sleep 6h
root         137  0.0  0.0   4132  1280 ?        S    04:31   0:00 /bin/bash /challenge/.init
root         138  0.0  0.0   4132  1280 ?        S    04:31   0:00 /bin/bash /challenge/.init
root         139  0.0  0.0   5204  3520 ?        S    04:31   0:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
root         140  0.0  0.0   2744  1280 ?        S    04:31   0:00 sleep 6h
root         141  0.0  0.0   2744  1600 ?        S    04:31   0:00 sleep 6h
hacker       142  0.4  0.0  13516  9280 ?        Ss   04:31   0:00 /usr/bin/python /challenge/decoy
hacker       144  0.4  0.0 231576  2880 pts/0    Ss   04:31   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-inte
hacker       150  0.0  0.0 231972  4160 pts/0    S    04:31   0:00 /run/dojo/bin/bash --login
hacker       160  0.0  0.0 233600  3840 pts/0    R+   04:31   0:00 ps aux
hacker@processes~killing-misbehaving-processes:~$ kill 142
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
^C
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{qR.ceGvWeliQbEIm8eKVgr4PvRLQd7ur1Vk1Ta6XUoBWIXc}
pwn.college{0G6NyVwn2JE4UO4jYQivTBdEi3DQs9bSllnhiJBCacaBT44}
pwn.college{PTiABZ0F-mpLDGslWGFE.NYa32Q36Yd-Gbjb459TE9YPInv}
pwn.college{OGuQbdVBr-Jdfl-K9P13kazw0YW9wOChsLOqdLwVxjlxKoO}
pwn.college{JtvbYGXGNBC8tgPnMOr7HjGijY-dLaVaFLiZnqiNthEN6wL}
. . .

hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{IaZ_E_g5cDShzYAa3qXgwsFVWNY.0FNzMDOxwiM5kjNzEzW}
```

## What I learned 
I learned that processes tha are being redirected into a file can also be killed to stop misbehaviour and find the desired result

## Incorrect tangents 
- After I killed the process, Some of the decoys were still piped into the named pipe and were taking time to get terminated, Since I was impatient I was onfued as to why it was not working

## References 
N/A
