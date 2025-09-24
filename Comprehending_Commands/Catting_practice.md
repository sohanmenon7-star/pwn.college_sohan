# Challenge 3 : Catting practice
This challenge is to improve your skills and concept of `cat` and wants you to use a complex absolute path to solve it without the use of `cd`

## My solve
**Flag:** `pwn.college{wXbVjrzMVIdttcumdi3EhDYOaPc.QXwITO0wiM5kjNzEzW}`

Since `cd` was not allowed, I directly put the absolute path given as the argument to solve the question
```
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /lib/tcltk/x86_64-linux-gnu/flag. Go cat it out **without** cding
into that directory!
hacker@commands~more-catting-practice:~$ cat /lib/tcltk/x86_64-linux-gnu/flag
pwn.college{wXbVjrzMVIdttcumdi3EhDYOaPc.QXwITO0wiM5kjNzEzW}
```

## What I learned 
I learnt how to use the `cat` command better, by practicing it with a difficult absolute path

## Incorrect tangents 
N/A

## References 
N/A
