# Challenge 4 : Grepping for a needle in a haystack
This challenge is about using `grep` to find a specific string within a text file

## My solve
**Flag:** `pwn.college{kAR-OP3F19Hrw2yjSwxn-5N3qcE.QX3EDO0wiM5kjNzEzW}`

To solve this challenge, as instructed, I invoked the `grep` command to find the flag. Since all flags start from 'pwn.college', I put that as the argument alongside the specified search location(absolute path) provided.
```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/date.txt
grep: /challenge/date.txt: No such file or directory
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data
grep: /challenge/data: No such file or directory
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{kAR-OP3F19Hrw2yjSwxn-5N3qcE.QX3EDO0wiM5kjNzEzW}
```

## What I learned 
The use of `grep` and how it can be useful when you have to find a specific text in large file

## Incorrect tangents 
N/A

## References 
N/A
