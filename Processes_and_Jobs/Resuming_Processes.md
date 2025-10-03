# Challenge 6 : Resuming Processes
To get to this flag, You need to run the program suspend it, and then resume it using `fg` builtin to obtain the flag

## My solve
**Flag:** `pwn.college{0y-vhRyV_gp3GZzt_-1V1p1EoMA.QX2QDO0wiM5kjNzEzW}`

As instructed, I simply ran /challenge/run, suspended it using `Ctrl-Z` and then resumed it using `fg` builtin as told in the challenge to get the flag
```
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{0y-vhRyV_gp3GZzt_-1V1p1EoMA.QX2QDO0wiM5kjNzEzW}
Don't forget to press Enter to quit me!

Goodbye!
```

## What I learned 
I learned how to resume programs using a builtin `fg`, since without this you might as well terminate any process you arent using

## Incorrect tangents 
N/A

## References 
N/A
