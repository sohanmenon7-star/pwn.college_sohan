# Challenge 4 : Changing Permissions 
This challenge teaches you about changing permissions using the command `chmod`

## My solve
**Flag:** `pwn.college{EtNL7KCEPhkSjpUrQTPGpeWb1_E.QXzcjM1wiM5kjNzEzW}`

- As told in the challenge, I used `chmod` to change permissions for /flag file
- I did this by giving the argument `go+r` to allow group owners and others to read the file /flag
```
hacker@permissions~changing-permissions:~$ chmod go+r /flag
hacker@permissions~changing-permissions:~$ cat/flag
bash: cat/flag: No such file or directory
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{EtNL7KCEPhkSjpUrQTPGpeWb1_E.QXzcjM1wiM5kjNzEzW}
```

## What I learned 
- I learned about the `chmod` and how it can be used to change permissions for a file/directory(Normally only usable by root as it has the `write` allowed for most files)
- I also learned how to read the access permission given in the `ls -l` description of a file

## Incorrect tangents 
N/A

## References 
N/A
