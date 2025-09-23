# Challenge 8 : Implicit relative paths
The challenge shows you how to use `.` to invoke a program in the current directory

## My solve
**Flag:** `pwn.college{Ei_qc50q0mE9hlryF389M3qf15O.QXxUTN0wiM5kjNzEzW}`

- Change directory to `/challenge` and after which input `./run` instead of just `run` as that will not be able to invoke the program
```
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ run
bash: run: command not found
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Ei_qc50q0mE9hlryF389M3qf15O.QXxUTN0wiM5kjNzEzW}
```

## What I learned 
I learnt the use case of `.` in commands and that Linux will avoid looking for 'naked' paths in a current directory
I also learnt what a 'naked' path is

## Incorrect tangents 
N/A

## References 
N/A
