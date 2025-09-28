# Challenge 3 : Appending outputs
This challenge is about using the append mode `>>` to append two outputs into a single file without using truncate `>` 

## My solve
**Flag:** `pwn.college{AvdZ8K29557YUUNaPnlCeviSsMQ.QX3ATO0wiM5kjNzEzW}` 

As explained in the challenge, I redirected the stdout using `>>` to ~/the-flag after which I simply `cat` ~/the-flag
```
hacker@piping~appending-output:~$ /challenge/run >> ~/the-flag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /home/hacker/the-flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] Good luck!

[TEST] You should have redirected my stdout to a file called /home/hacker/the-flag. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
I will write the flag in two parts to the file /home/hacker/the-flag! I'll do
the first write directly to the file, and the second write, I'll do to stdout
(if it's pointing at the file). If you redirect the output in append mode, the
second write will append to (rather than overwrite) the first write, and you'll
get the whole flag!
hacker@piping~appending-output:~$ cat ~/the-flag
 |
\|/ This is the first half:
 v
pwn.college{AvdZ8K29557YUUNaPnlCeviSsMQ.QX3ATO0wiM5kjNzEzW}
                              ^
     that is the second half /|\
                              |

If you only see the second half above, you redirected in *truncate* mode (>)
rather than *append* mode (>>), and so the write of the second half to stdout
overwrote the initial write of the first half directly to the file. Try append
mode!
```

## What I learned 
- I learnt about append mode `>>` and how it redirects output to a file similar to truncate `>`
- Unlike `>` however which overides the first output, `>>` appends bith output and therefore reading the file will give both outputs not just one.

## Incorrect tangents 
N/A

## References 
N/A
