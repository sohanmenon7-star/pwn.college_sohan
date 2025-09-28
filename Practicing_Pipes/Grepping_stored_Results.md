# Challenge 6 : Grepping stored results
Challenge 6 is about combining the concept of grep and redirection
The challenge asks you to redirect output to a file and then use `grep` to find the flag
## My solve
**Flag:** `pwn.college{MzZoacYgRsSAow3MmQk-wKvwkOx.QX4EDO0wiM5kjNzEzW}` 

- In the challenge it has been told to redirect the output of /challenge/run to /tmp/data.txt which I did by using the truncate `>`
- After this, I used `grep` to find the flag by putting the argument as 'pwn' and path of the file /tmp/data.txt, This gave me the flag
```
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep pwn /tmp/data.txt
pwns
pwned
pwning
pwn.college{MzZoacYgRsSAow3MmQk-wKvwkOx.QX4EDO0wiM5kjNzEzW}
pwn
```

## What I learned 
I learned about using complex problem solving by using both `grep` and redirection to solve complicated to questions and find specific output in a large output file

## Incorrect tangents 
N/A

## References 
N/A
