# Challenge 1 : Redirecting outputs
This challenge teaches you about redirecting standard output to specific file using `>` to redirect an output to a file

## My solve
**Flag:** `pwn.college{s1VRvjmbT_aEyiy6UiJXyTrhJOP.QX0YTN0wiM5kjNzEzW}` 

As told in the challenge, I used the `echo` command to give the out PWN and redirect it to file COLLEGE using `>`
```
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your
flag:
pwn.college{s1VRvjmbT_aEyiy6UiJXyTrhJOP.QX0YTN0wiM5kjNzEzW}
```

## What I learned 
I learnt about the three channels of communication namely, stdin, stdout, stderr.
In this challenge I leanrt about redirecting standard output to a file using `>`

## Incorrect tangents 
N/A

## References 
N/A
