# Challenge 2 : Setting PATH
In this challenge you have to set a specific PATH as mentioned and only then will a command run to give you the flag

## My solve
**Flag:** `pwn.college{EC5kARG5kbZHt_K1NrTNF4O6eNY.QX1cjM1wiM5kjNzEzW}`

As told, I assigned `PATH=/challenge/more_commands/` whic housed the `win` command, then on running the program, it was successfully able to invoke `win` to give me the flag
```
hacker@path~setting-path:~$ PATH=/challenge/more_commands/
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{EC5kARG5kbZHt_K1NrTNF4O6eNY.QX1cjM1wiM5kjNzEzW}
```

## What I learned 
I learned you can set a specific PATH for commands that would normally not have been invoked

## Incorrect tangents 
N/A

## References 
N/A
