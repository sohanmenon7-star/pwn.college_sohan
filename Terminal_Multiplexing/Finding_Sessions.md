# Challenge 3 : Finding Sessions
In this challenge, there are multiple detatched terminals, you have to find the flag by reattaching them one by one to find the flag

## My solve
**Flag:** `pwn.college{4HzHl4uGCvKRbcLygMyPXb8Y9VC.01N4IDOxwiM5kjNzEzW}`

- As told in the challenge, I sued `screen -ls` to see the teminals detached
- I then reattached them one by one to search for the flag, eventually I got the flag
```
hacker@terminal-multiplexing~finding-sessions:~$ screen -ls
There are screens on:
        144.session_63bb98820ce67122    (Detached)
        147.session_a58221c05f415b68    (Detached)
        150.session_85fa5bd5440ae130    (Detached)
3 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_63bb98820ce67122
[detached from 144.session_63bb98820ce67122]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_a58221c05f415b68
[detached from 147.session_a58221c05f415b68]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_85fa5bd5440ae13

hacker@terminal-multiplexing~finding-sessions:~$  echo 'Congratulations! You found the right session!'
Congratulations! You found the right session!
hacker@terminal-multiplexing~finding-sessions:~$  echo pwn.college{4HzHl4uGCvKRbcLygMyPXb8Y9VC.01N4IDOxwiM5kjNzEzW}
pwn.college{4HzHl4uGCvKRbcLygMyPXb8Y9VC.01N4IDOxwiM5kjNzEzW}
hacker@terminal-multiplexing~finding-sessions:~$
```

## What I learned 
- I learned that `screen -ls` to see the terminals running in the background
- Also you can reattach a specific terminal by giving its name in the argument

## Incorrect tangents 
N/A

## References 
N/A
