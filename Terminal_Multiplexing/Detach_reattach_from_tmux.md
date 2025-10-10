# Challenge 5 : Detached and reattached from tmux
Similar to preious challenges, you have to use tmux to open a new terminal, detatch and then reattach it

## My solve
**Flag:** `pwn.college{YlDIzWzaRCt9g1q-NpbvQZq4UsL.0VO4IDOxwiM5kjNzEzW}`

- I used `tmux` to open a terminal and then detach from it using Ctrl-B d
- I ran the program /challenge/run and then reattached using `tmux a` to get the flag
```
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux
[detached (from session 0)]
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ /challenge/run
Found detached tmux session: 0
Sending flag to your tmux session...

Flag sent! Now reattach to your tmux session with:
  tmux attach

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux a

hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$  echo Congratulations, here is your flag: pwn.college{YlDIzWzaRCt9g1q-NpbvQZq4UsL.0VO4IDOxwiM5kjNzEzW}
Congratulations, here is your flag: pwn.college{YlDIzWzaRCt9g1q-NpbvQZq4UsL.0VO4IDOxwiM5kjNzEzW}
```

## What I learned 
- I learned a more modern way of opening another terminal using `tmux`
- Its keyboard shortcuts are Ctrl B instead of the usual Ctrl A

## Incorrect tangents 
N/A

## References 
N/A
