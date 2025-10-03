# Challenge 9 : Starting Background Processes
In this challenge, you have to directly background a process instead of suspending it first 
## My solve
**Flag:** `pwn.college{AnB35B4lElqOmVwK0i_wdm4G2B3.QX5QDO0wiM5kjNzEzW}`

As explained, I ran the challenge with `&` as the argument to directly background the process instead of first suspending it
```
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 138
hacker@processes~starting-backgrounded-processes:~$


Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{AnB35B4lElqOmVwK0i_wdm4G2B3.QX5QDO0wiM5kjNzEzW}
```

## What I learned 
I learnt about directly backgrounding characters by putting `&` as the argument when launching a process, this saves a lot of time and effort by notneeding you to first suspend it first

## Incorrect tangents 
N/A

## References 
N/A
