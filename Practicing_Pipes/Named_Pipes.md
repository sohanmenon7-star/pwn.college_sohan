# Challenge 14 : Named Pipes
This challenge asked you to create a named pipe (fifo) and redirect the stdout of a program into it

## My solve
**Flag:** `pwn.college{Mz-qn-YJzqIRKxcvBB6xN3xc10t.01MzMDOxwiM5kjNzEzW}`

- As explained in the challenge, I firstly created a named pipe /tmp/flag_file using the `mkfifo` command
- After this I redirected the stdout of /challenge/run into the fifo using `>`
- This opened the write mode of FIFO which will be blocked as both wirte and read mode need to be open for it to run
- As it was not working when I ran `cat /tmp/flag_file` in the same terminal
- I opened another termninal and ran `cat /tmp/flag_file` to obtain the flag
```
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at 
/tmp/flag_fifo! Here is your flag:
pwn.college{Mz-qn-YJzqIRKxcvBB6xN3xc10t.01MzMDOxwiM5kjNzEzW}
```

## What I learned 
- I learned about named pipes(also called fifo) which are persistent name files as opposed to the temporary named pipes created by process substitution
- I can create these fifo with the command `mkfifo` and give the name of the fifo as an argument
- Similar to named pipes, I can redirect stdout into this fifo from a program

## Incorrect tangents 
N/A

## References 
N/A
