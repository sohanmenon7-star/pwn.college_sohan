# Challenge 7 : Explicit relative paths
The challenge instructs you to use `.` to use relative paths

## My solve
**Flag:** `pwn.college{sGOyjnEfmt9JdpMlR4qFAZGfs34.QXwUTN0wiM5kjNzEzW}`

As told in the challenge, change directories to `/` and then use `.` before the path to solve the challenge
```
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{sGOyjnEfmt9JdpMlR4qFAZGfs34.QXwUTN0wiM5kjNzEzW}
```

## What I learned 
I learnt about `.` and `..`, which mean current directory and parent directory respectively and how to use them in commands to understand paths better

## Incorrect tangents 
N/A

## References 
N/A
