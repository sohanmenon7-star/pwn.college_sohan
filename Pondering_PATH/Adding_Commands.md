# Challenge 4 : Adding Commands
In this challenge, `win` does not exist you need to create a shell script and modify the PATH so `win` can be executed

## My solve
**Flag:** `pwn.college{obw0znxK9X_ZTGcAdjPFmzvWH-R.QX2cjM1wiM5kjNzEzW}`

- I started off by creating win using `touch` and then wrote the shell script in it by providing the absolute path of `cat` to /flag
- I found the absolute path by using `which cat`
- I granted permission for win to be executable
- Changed PATH to /home/hacker since that is where `win` was created
- I then ran the program
```
hacker@path~adding-commands:~$ touch win
hacker@path~adding-commands:~$ nano win
hacker@path~adding-commands:~$ which cat
/run/dojo/bin/cat
hacker@path~adding-commands:~$ chmod ugo+x /flag
chmod: changing permissions of '/flag': Operation not permitted
hacker@path~adding-commands:~$ chmod ugo+x win
hacker@path~adding-commands:~$ PATH=/home/hacker/
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{obw0znxK9X_ZTGcAdjPFmzvWH-R.QX2cjM1wiM5kjNzEzW}
```

## What I learned 
I learned you can 'add' commands to PATH or use absolute paths of a command in case PATH was changed

## Incorrect tangents 
N/A

## References 
N/A
