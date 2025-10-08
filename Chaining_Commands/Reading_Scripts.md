# Challenge 12 : Reading Shell scripts
In this challenge you need to read a shell script to get the password and run the shell script correctly to obtain the flag

## My solve
**Flag:** `pwn.college{MpokQI8aZcyUGJ43gO50aJZAlLE.0lMwgDOxwiM5kjNzEzW}`

- As told, I used `cat` to read the script to see the password
- After which, I simply used the shell script to understand what to do to get the flag
```
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run 
hack the PLANET
CORRECT! Your flag:
pwn.college{MpokQI8aZcyUGJ43gO50aJZAlLE.0lMwgDOxwiM5kjNzEzW}
```

## What I learned 
I learnt you can read shell scripts by simply `cat`ing them, this can help tremendously when trying to understand why a function does what it does

## Incorrect tangents 
N/A

## References 
N/A
