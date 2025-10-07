# Challenge 5 : Redirecting Script output
In this challenge you simply have to redirect stdout of x.sh into a command /challenge/solve

## My solve
**Flag:** `pwn.college{E8jIf3BzqArs4fgyPzaV3L3ze-G.QX4ETO0wiM5kjNzEzW}`

- I created a shell script using `touch x.sh`
- I used `echo "/challenge/pwn; /challenge/college > x.sh"` to write the chain of commands to x.sh
- I then used `bash x.sh | /challenge/solve` to redirect the stdout of shell script into command to get the flag
```
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~redirecting-script-output:~$ echo "/challenge/pwn; /challenge/college" > x.sh
hacker@chaining~redirecting-script-output:~$ cat x.sh
/challenge/pwn; /challenge/college
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{E8jIf3BzqArs4fgyPzaV3L3ze-G.QX4ETO0wiM5kjNzEzW}
```

## What I learned 
I learned how to redirect stdout of a shell script into a command by using the basic pipings taught in earlier modules

## Incorrect tangents 
I originally had not written /challenge/pwn and /challenge/college in the same line which gave me an error

## References 
N/A
