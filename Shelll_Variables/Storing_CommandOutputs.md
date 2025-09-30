# Challenge 6 : Storing Command Outputs
This challenge teaches you about storing outputs of programs in variables using `$()`

## My solve
**Flag:** `pwn.college{wb7RmoxP2Voy24_Asn0NqZmKodq.QX1cDN1wiM5kjNzEzW}`

As told in the challenge I first stored the output of /challenge/run into PWN using `=$()`
After which I simply used `echo` to print the flag
```
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{wb7RmoxP2Voy24_Asn0NqZmKodq.QX1cDN1wiM5kjNzEzW}
```

## What I learned 
I learnt that when needed to, You can store outputs into variables for future use by `variable=$(command)`
This is called Command Substitution

## Incorrect tangents 
N/A

## References 
N/A
