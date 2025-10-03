# Challenge 7 : Resuming Processes
In this challenge, You have to run a program, suspend it, and then begin running it in the background and then run it again to get the flag

## My solve
**Flag:** `pwn.college{k6sC462eR49TYDkk6gYKBjTsWDq.QX3QDO0wiM5kjNzEzW}`

- As told, I ran /challenge/run, suspended it using `Ctrl-Z` and then run it in the background with `bg`
- Then I simply restrated /challenge/run to get the flag 
```
hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         139 S+   bash /challenge/run
root         141 R+   ps -o user=UID,pid,stat,cmd

I don't see a second me!

To pass this level, you need to suspend me, resume the suspended process in the
background, and then launch a new version of me! You can background me with
Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to
do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~backgrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~backgrounding-processes:~$


Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out.

hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         139 S    bash /challenge/run
root         149 S    sleep 6h
root         150 S+   bash /challenge/run
root         152 R+   ps -o user=UID,pid,stat,cmd

Yay, I found another version of me running in the background! Here is the flag:
pwn.college{k6sC462eR49TYDkk6gYKBjTsWDq.QX3QDO0wiM5kjNzEzW}

Goodbye!
```

## What I learned 
I learned how to resume programs using a builtin `fg`, since without this you might as well terminate any process you arent using

## Incorrect tangents 
N/A

## References 
N/A
