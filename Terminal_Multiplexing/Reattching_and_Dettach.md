# Challenge 2 : Detatch and reattach
This challenge teaches you to dettach and reattach from a terminal to obtain the flag

## My solve
**Flag:** `pwn.college{Adi4GaURcOZ0Oc6OOLAoYyAOwWS.0lN4IDOxwiM5kjNzEzW}`

- As explained in the challenge, I simply used `screen` to open another terminal and then `Ctrl-A` then `d` to dettach from the terminal
- After which I ran /challenge/run and then reattached the terminal using `screen -r` to get the flag
```
hacker@terminal-multiplexing~detaching-and-attaching:~$
hacker@terminal-multiplexing~detaching-and-attaching:~$ echo Yes! Flag is: pwn.college{Adi4GaURcOZ0Oc6OOLAoYyAOwWS.0lN4IDOxwiM5kjNzEzW}
Yes! Flag is: pwn.college{Adi4GaURcOZ0Oc6OOLAoYyAOwWS.0lN4IDOxwiM5kjNzEzW}

hacker@terminal-multiplexing~detaching-and-attaching:~$ screen
[detached from 140.pts-0.terminal-multiplexing~detaching-and-attaching]
hacker@terminal-multiplexing~detaching-and-attaching:~$ /challenge/run
Found detached screen session: 140.pts-0.terminal-multiplexing~detaching-and-attaching
Sending flag to your screen session...

Flag sent! Now reattach to your screen session with:

  screen -r

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen -r
[screen is terminating]
```

## What I learned 
- I learned you can reattach and dettach from a terminal by pressing Ctrl-A and then d
- You can reattach to that terminal when you use `screen -r`

## Incorrect tangents 
N/A

## References 
N/A
