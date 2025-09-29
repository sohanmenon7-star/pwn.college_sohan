
# Challenge 8 : Grepping Errors
The challenge asks you to `grep` the standard error to find the flag using the `>&` operator
## My solve
**Flag:** `pwn.college{cYzWKCr17xC_QzA1I9NI4xl-IdA.QX1ATO0wiM5kjNzEzW}` 

The challegne gave information on how to use `>&` to combine the stderr and stdout of a program
Using which I put the `2>&1` operator to combine them and then used the `|` operator to `grep` and find the flag
```
hacker@piping~grepping-errors:~$ /challenge/run 2>&1 | grep pwn
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwned
pwn.college{cYzWKCr17xC_QzA1I9NI4xl-IdA.QX1ATO0wiM5kjNzEzW}
pwn
pwning
pwns
pwn
```

## What I learned 
- I Learnt about the use of `>&` operator and how it can be used to combine the standard error and standard output
- This is needed as `|` operator can only redirect stdout (`2|` does not exist
)
## Incorrect tangents 
N/A

## References 
N/A
