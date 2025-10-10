# Challenge 6 : Switching_Windows with tmux
In this challenge, you have to switch windows using keyboard shortcuts in tmux instead of screen

## My solve
**Flag:** `pwn.college{w2hBtbKa1p-6EVJUUEVXPWqZe7B.0FM5IDOxwiM5kjNzEzW}`

- I simply used `tmux a` to open the termninal with windows in it
- I then used the keyboard shortcut Ctrl-B n to switch the next window
```
hacker@terminal-multiplexing~switching-windows-tmux:~$ tmux a
[detached (from session challenge_session)]

 cat <<MSG
Welcome to the tmux window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-B 0 to switch to window 0!
MSG
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Welcome to the tmux window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-B 0 to switch to window 0!
> MSG
Welcome to the tmux window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-B 0 to switch to window 0!

hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{w2hBtbKa1p-6EVJUUEVXPWqZe7B.0FM5IDOxwiM5kjNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{w2hBtbKa1p-6EVJUUEVXPWqZe7B.0FM5IDOxwiM5kjNzEzW}
```

## What I learned 
I learned that there can be multiple windows open in a terminal with tmux and I learned about the keyboard shortcuts to manipulate the windows

## Incorrect tangents 
N/A

## References 
N/A
