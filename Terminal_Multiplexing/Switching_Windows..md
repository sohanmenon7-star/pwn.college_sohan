# Challenge 4 : Switching_Windows
In this challenge, you have to switch windows using keyboard shortcuts

## My solve
**Flag:** `pwn.college{cUUKKaHxfshKKSLcBkQWZyZ5LVf.0FO4IDOxwiM5kjNzEzW}`

- I simply used `screen -r` to open the termninal with windows in it
- I then used the keyboard shortcut Ctrl-A n to switch the next windows
```
hacker@terminal-multiplexing~switching-windows:~$ screen -ls
There are screens on:
        144.session_63bb98820ce67122    (Remote or dead)
        147.session_a58221c05f415b68    (Remote or dead)
        150.session_85fa5bd5440ae130    (Remote or dead)
        136.challenge_session   (Detached)
4 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~switching-windows:~$ screen -r
[screen is terminating]

 cat <<MSG
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
MSG
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Welcome to the window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-A 0 to switch to window 0!
> MSG
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!

hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{cUUKKaHxfshKKSLcBkQWZyZ5LVf.0FO4IDOxwiM5kjNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{cUUKKaHxfshKKSLcBkQWZyZ5LVf.0FO4IDOxwiM5kjNzEzW}
```

## What I learned 
I learned that there can be multiple windows open in a terminal and I learned about the keyboard shortcuts to manipulate the windows

## Incorrect tangents 
N/A

## References 
N/A
