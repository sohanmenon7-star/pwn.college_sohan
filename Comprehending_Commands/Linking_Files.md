# Challenge 14 : Linking Files
This challenge forces you to use a symlink to read the file containing the flag, as if you try to use `cat` the permission will be denied

## My solve
**Flag:** `pwn.college{QR6SetY55aw7bWxpZzrzvNWYSHS.QXxMDO0wiM5kjNzEzW}`

- This challenge has given us some points of information, 1. the flag is '/flag' 2. '/challenge/catflag' will read '~/not-the-flag' 3. Directly trying to open '/flag' will not be allowed
- Using this information, I created a link with the name '~/not-the-flag' using the `ln -s` command providing the '/flag' as the absolute path(The location)
- Doing this tricked it into giving the flag
```
hacker@commands~linking-files:~$ ln -s /flag ~/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{U9iI1ozCMomeCmdBUA_tOFgM_al.QX5ETN1wiM5kjNzEzW}
```

## What I learned 
I learnt how to use the `ln -s` command to create a link to specified path and give it a name. I also learnt the links are actually files that redirect you to a different file

## Incorrect tangents
- I tried directly created a link to '/flag' which upon running denied me permission 
- After this I also tried creating a link from /challenge/not-the-flag to /flag which also did not work since /challenge/not-the-flag already exists

## References
N/A
