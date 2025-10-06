# Challenge 2 : Groups and Files
This challenge asks you to change group ownership to read it by using `chgrp`

## My solve
**Flag:** `pwn.college{gYgjW1js_bo3zGUxAsBp6xDf8y6.QXxcjM1wiM5kjNzEzW}`

As told in the challegne, I simply used `chgrp` with hacker and /flag as arguments to change group ownerships and then read the /flag file
```
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{gYgjW1js_bo3zGUxAsBp6xDf8y6.QXxcjM1wiM5kjNzEzW}
```

## What I learned 
- I learned about group ownership and how it can be changed using `chgrp`
- I also learned a user can read the groups he is in by using `id`

## Incorrect tangents 
N/A

## References 
N/A
