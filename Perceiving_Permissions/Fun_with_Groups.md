# Challenge 3 : Fun with Groups 
Similar to the previous challenge, you are supposed to change group ownership of the flag file but this time to seperate a group

## My solve
**Flag:** `pwn.college{47_FaQwKKIeDYxEK8FYvLpDQpvG.QXycjM1wiM5kjNzEzW}`

As explained in the challenge, I used `id` to find the group hacker user is in and then similar to the previous challenge I changed group ownership and then read the /flag file
```
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp14714) groups=1000(grp14714)
hacker@permissions~fun-with-groups-names:~$ chgrp grp14714 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{47_FaQwKKIeDYxEK8FYvLpDQpvG.QXycjM1wiM5kjNzEzW}
```

## What I learned 
I learned more about groups that a user can be in and how to check it using `id`

## Incorrect tangents 
N/A

## References 
N/A
