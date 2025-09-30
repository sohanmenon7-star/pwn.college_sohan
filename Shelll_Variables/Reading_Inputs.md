# Challenge 7 : Reading Inputs
This challenge asks you to input the values of a variable in the shell by providing it with stdin using `read`

## My solve
**Flag:** `pwn.college{wb7RmoxP2Voy24_Asn0NqZmKodq.QX1cDN1wiM5kjNzEzW}`

As explained in the challenge I used `read` with argument PWN vairable to accept input from the user and setting the value as COLLEGE. This gave me the flag
```
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{wb7RmoxP2Voy24_Asn0NqZmKodq.QX1cDN1wiM5kjNzEzW}
```

## What I learned 
- I learnt that `read` can be used to accept input from the user and assign it to a variable
- Also, `read` can be upgraded by adding `-p` to it to specify a prompt

## Incorrect tangents 
N/A

## References 
N/A
