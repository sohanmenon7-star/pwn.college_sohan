# Challenge 1 : Listing Processes
In this challenge you simply need to list all launched processes using the `ps aux` command and find the filename containing the flag

## My solve
**Flag:** `pwn.college{AFWzSmKRY9aU_gLJCKvQtMYoBIu.QX4MDO0wiM5kjNzEzW}`

- As explained in the challenge, the process was already launched and this I simply used `ps aux` (or `ps -ef`) to obtain all running programs and their location
- After relaunching the program, I obtained the flag
```
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   03:49   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-works
root           7  0.0  0.0 231708  2560 ?        S    03:49   0:00 /run/dojo/bin/sleep 6h
root         132  0.0  0.0   4132  2560 ?        S    03:49   0:00 /challenge/5818-run-4957
root         135  0.0  0.0   2744  1600 ?        S    03:49   0:00 sleep 6h
hacker       137  0.0  0.0 231576  3520 pts/0    Ss   03:49   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-inte
hacker       143  0.0  0.0 231940  4160 pts/0    S    03:49   0:00 /run/dojo/bin/bash --login
hacker       163  0.0  0.0 231944  4160 pts/0    S    03:54   0:00 /run/dojo/bin/bash --login
hacker       175  0.0  0.0 233600  3840 pts/0    R+   03:54   0:00 ps aux
hacker@processes~listing-processes:~$ /challenge/5818-run-4957
Yahaha, you found me! Here is your flag:
pwn.college{AFWzSmKRY9aU_gLJCKvQtMYoBIu.QX4MDO0wiM5kjNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').
```

## What I learned 
- I learnt about processes, what they are and how to list them using `ps`
- `ps` is old, therefore to use it more effectively, You need to use `ps aux` which lists every program running or not and shows their location file as well


## Incorrect tangents 
- I used `ps -e` which did not give me all the information needed

## References 
N/A
