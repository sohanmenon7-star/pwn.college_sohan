# Challenge 1 : Launhcing Screen
Challenge 1 is about using `screen` command to open another terminal inside the terminal

## My solve
**Flag:** `pwn.college{Uw79uI9o5HTC7Ze67Gihi_N849D.0VN4IDOxwiM5kjNzEzW}`

- As explained in the challenge, I simply used `screen` to open another terminal which had the flag
```
hacker@terminal-multiplexing~launching-screen:~$ screen
[screen is terminating]
Congratulations! You're inside a screen session!
Here's your flag:
pwn.college{Uw79uI9o5HTC7Ze67Gihi_N849D.0VN4IDOxwiM5kjNzEzW}
hacker@terminal-multiplexing~launching-screen:~$
```

## What I learned 
- This challenge taught me about `screen` which can be used to open another terminal within a terminal
- To exit this terminal, press Ctrl-d or `exit` in command line

## Incorrect tangents 
N/A

## References 
N/A
