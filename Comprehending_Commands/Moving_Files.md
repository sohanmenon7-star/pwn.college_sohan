# Challenge 9 : Moving Files
The challenge requires you to move the file from one place to the desired location

## My solve
**Flag:** `pwn.college{skfBkgQb26WU-3C4BZ-rpjed-6L.0VOxEzNxwiM5kjNzEzW}`

The challenge gave you the absolute path of the location you needed to move the file to, using that as the argument to `mv` command, I obtained the flag
```
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{skfBkgQb26WU-3C4BZ-rpjed-6L.0VOxEzNxwiM5kjNzEzW}
```

## What I learned 
I learnt how to move files from one location to another by using the `mv` command and the path as the argument

## Incorrect tangents 
N/A

## References 
N/A
