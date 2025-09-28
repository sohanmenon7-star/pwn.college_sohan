# Challenge 7 : Grepping live output
This challenge teaches you about the pipe operator `|` and how to grep files with creating a seperate file of output

## My solve
**Flag:** `pwn.college{MzZoacYgRsSAow3MmQk-wKvwkOx.QX4EDO0wiM5kjNzEzW}` 

- As instructed in the challenge, I simply used `|` to solve this challenge
- To the left of `|` I ran the program and to its right I used `grep` with the string pwn to find the flag
```
hacker@piping~grepping-live-output:~$ /challenge/run | grep pwn
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{YYx_20g63mX9kBO0vzFGDzGEvX0.QX5EDO0wiM5kjNzEzW}
pwning
pwned
pwns
pwn
```

## What I learned 
I found about the pipe operator `|` and how it can be used to specify outputs depending on the command put to the right of it.
This saves a lot of time by not creating a seperate output file and 'cutting the middle man'

## Incorrect tangents 
N/A

## References 
N/A
