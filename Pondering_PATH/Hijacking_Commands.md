# Challenge 5 : Hijacking Commands
This challenge is about Hijacking the `rm` command so it can `cat` the flag once given permission

## My solve
**Flag:** `pwn.college{Ue4tKyzagSsh2sjK_mO2AKPK6sn.QX3cjM1wiM5kjNzEzW}`

- I started by creating an `rm` script and writing the absolute path of `cat` command in it so it will read the flag
- Gave permission to `rm`
- Set PATH to /home/hacker/
- Ran /challenge/run to get the flag
```
hacker@path~hijacking-commands:~$ touch rm
hacker@path~hijacking-commands:~$ nano
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ which cat
/run/dojo/bin/cat
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ chmod ugo+x rm
hacker@path~hijacking-commands:~$ PATH=/home/hacker/
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{Ue4tKyzagSsh2sjK_mO2AKPK6sn.QX3cjM1wiM5kjNzEzW}
```

## What I learned 
I learnt that you can hijack commands by creating a command with the same name and changing the PATH such that only the new command is accessible

## Incorrect tangents 
N/A

## References 
N/A
