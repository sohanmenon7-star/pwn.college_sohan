# Challenge 2 : Redirecting more outputs
This challenge expands on the concept of redirecting output to files by forcing you to use `>` to obtain the flag

## My solve
**Flag:** `[FLAG] pwn.college{oVQ0NR3kAc5yzTXsjKSyO72SstQ.QX1YTN0wiM5kjNzEzW}` 

As instructed in the challenge, I used `>` to redirect the output of /challenge/run to file myflag and then `cat` to obtain the flag
```
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{oVQ0NR3kAc5yzTXsjKSyO72SstQ.QX1YTN0wiM5kjNzEzW}
```

## What I learned 
I learnt in depth about how to use `>` to redirect stdout to files by practicing it more in the challenge

## Incorrect tangents 
N/A

## References 
N/A
