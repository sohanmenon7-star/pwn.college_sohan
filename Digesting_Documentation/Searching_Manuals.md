# Challenge 4 : Searching Manuals
This challnge is about searching large manuals for the desired description using `/` followed by desired string and `n`,`N` to move between finds

## My solve
**Flag:** `pwn.college{sgn4L2ufGrRnQaBLoduvgFoxmP9.QX1EDO0wiM5kjNzEzW}`

As explained in the challenge, I opened the manual of `challenge` and then used `/flag` to search for the argument containing the flag.
After this I simply used `n` to browse through all the strings till I found the argument
```
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --hi
Initializing...
Correct usage! Your flag: pwn.college{sgn4L2ufGrRnQaBLoduvgFoxmP9.QX1EDO0wiM5kjNzEzW}
```

## What I learned 
This problem taught me about searching manuals using `/`,`n`,`N`,`?` for a desired part of the manual when it is too long

## Incorrect tangents 
N/A

## References 
N/A
