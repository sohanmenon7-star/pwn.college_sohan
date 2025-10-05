# Challenge 3 : Cracking passwords
This challenge asks you to crack the password of zardus and then `su` into it and then run a program to find the flag

## My solve
**Flag:** `pwn.college{ozosOa2ZTbumoVmTnFrLNZoMIVk.QX3UDN1wiM5kjNzEzW}`

- As instructed, I first used `john` with /challenge/shadow-leak as the argument to crack the passwords of the leaked zardus hash
- After waiting for the decryption I obtained the password and then used `su` to change to zardus
- I put the password, ran /challenge/run and got the flag
```
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04965g/s 289.1p/s 289.1c/s 289.1C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ --show
bash: --show: command not found
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{ozosOa2ZTbumoVmTnFrLNZoMIVk.QX3UDN1wiM5kjNzEzW}
```

## What I learned 
- I learnt about the `john` command and how it can be used to crack passwords of leaked hashes of users
- These hashes can be found in /etc/shadow 

## Incorrect tangents 
N/A

## References 
N/A
