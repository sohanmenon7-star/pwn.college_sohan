# Challenge 8 : SUID bit
In this challenge, asks you to set SUID for a program to change the user to root and then execute the program without the need of a password

## My solve
**Flag:** `pwn.college{4FcqU4s-7XEE_nMxD2BRTWQqKoc.QXzEjN0wiM5kjNzEzW}`

- As explained in the challenge, I used `chmod u+s /challenge/pwn` to give the SUID to the /challenge/pwn program
- After running I was given the root shell, After I which read the flag file
```
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{4FcqU4s-7XEE_nMxD2BRTWQqKoc.QXzEjN0wiM5kjNzEzW}
```

## What I learned 
- I learnt about SUID(Set User ID), which gives the user root shell without a password
- This can be done by giving user `s` in `chmod` to a special program

## Incorrect tangents 
N/A

## References 
N/A
