# Challenge 4 : Handling Failure
In this challenge you are to create a shell script and then write the commands in it and then use `bash` to run the shell script to get the flag

## My solve
**Flag:** `pwn.college{45-zI4mnq_oUich0D9rCuu3tsJ7.QXxcDO0wiM5kjNzEzW}`

- I created a shell script using `touch x.sh`
- I used `echo /challenge/pwn > x.sh` and `echo /challenge/college >> x.sh` to write the commands in x.sh
- I then used `bash` to run x.sh as a shell script
```
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~your-first-shell-script:~$ echo /challenge/pwn > x.sh
hacker@chaining~your-first-shell-script:~$ cat x.sh
/challenge/pwn
hacker@chaining~your-first-shell-script:~$ echo /challenge/college >> x.sh
hacker@chaining~your-first-shell-script:~$ cat x.sh
/challenge/pwn
/challenge/college
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{45-zI4mnq_oUich0D9rCuu3tsJ7.QXxcDO0wiM5kjNzEzW}
```

## What I learned 
- This challenge taught me how to create a shell script, by put `.sh` after the filename
- To then run this shell script there is a special command, `bash` followed by the shell script

## Incorrect tangents 
I tried redirecing the stdout of the commands into x.sh which did not work

## References 
N/A
