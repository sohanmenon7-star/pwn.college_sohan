# Challenge 10 : Hidden Files
This challenge wants you to list hidden files present in a directory

## My solve
**Flag:** `pwn.college{I3uWZP5GcWiZ8rhHtLfxPsUR7nY.QXwUDO0wiM5kjNzEzW}`

As the challenge instructes, using the `ls -a` command will provide all files including hidden files
```
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-279302200611935  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-279302200611935
pwn.college{I3uWZP5GcWiZ8rhHtLfxPsUR7nY.QXwUDO0wiM5kjNzEzW}
```

## What I learned 
- I learnt that adding `.` in front of file will make it a hidden file, which is not a visible when using the `ls` command
- To find the hidden files, the `-a` needs to be added after the `ls` command

## Incorrect tangents
N/A

## References
N/A
