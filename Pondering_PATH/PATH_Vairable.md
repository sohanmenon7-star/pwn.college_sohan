# Challenge 1 : PATH Variable
The program in this challenge tries to delete the flag and you are to prevent it from removing the command to get the flag

## My solve
**Flag:** `pwn.college{YVo0qCh8M-8Ohw6bWWT8EQQfx8K.QX2cDM1wiM5kjNzEzW}`

As told, I assigned teh path variable `PATH=" "` so the command `rm` does not work, preventing it from removing the flag
```
hacker@path~the-path-variable:~$ PATH=" "
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: command not found
The flag is still there! I might as well give it to you!
pwn.college{YVo0qCh8M-8Ohw6bWWT8EQQfx8K.QX2cDM1wiM5kjNzEzW}
```

## What I learned 
I learned about the PATH Variable and how all bare commmand names use this vairable to access there functions and execute it

## Incorrect tangents 
N/A

## References 
N/A
