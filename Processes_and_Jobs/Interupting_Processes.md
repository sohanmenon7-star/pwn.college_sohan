# Challenge 3 : Interupting Processes
This challenge teaches you about interupting programs by pressing `Ctrl-C` and requires you to interupt a program to obtain the flag

## My solve
**Flag:** `pwn.college{Q6I2RxPMtWcrJo3ONqWz7xS_6nA.QXzQDO0wiM5kjNzEzW}`

- As told in the challenge, I simply ran the /challenge/run command and foreced it to exit by pressing `Ctrl-C`
```
hacker@processes~interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember,
you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:
pwn.college{Q6I2RxPMtWcrJo3ONqWz7xS_6nA.QXzQDO0wiM5kjNzEzW}
```

## What I learned 
I learned about interupting programs that are waiting for input from the terminal using `Ctrl-C`

## Incorrect tangents 
N/A

## References 
N/A
