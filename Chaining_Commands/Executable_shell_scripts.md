# Challenge 6 : Executable Shell Scripts
This challenge requires you to run a shell script without using `bash`

## My solve
**Flag:** `pwn.college{Q0kv-cJUR0j81vDEIKtPWduWwlJ.QX0cjM1wiM5kjNzEzW}`

- I started off by touching a script.sh and write /challenge/solve in it using `nano` 
- After which I gave script.sh permission to execute and then simply called its absolute path
```
hacker@chaining~executable-shell-scripts:~$ touch script.sh
hacker@chaining~executable-shell-scripts:~$ nano script.sh
hacker@chaining~executable-shell-scripts:~$ chmod ugo+x script.sh
hacker@chaining~executable-shell-scripts:~$ ./script.sh
Congratulations on your shell script execution! Your flag:
pwn.college{Q0kv-cJUR0j81vDEIKtPWduWwlJ.QX0cjM1wiM5kjNzEzW}
```

## What I learned 
- I learned that you can run a shell script without the use of `bash` by making the script executable

## Incorrect tangents 
I used `~/script.sh` to call the script but there was another directory named `~` which is why I was getting an error

## References 
N/A
