# Challenge 3 : Matching with []
The challenge wants you to use the glob `[]` to change directory and using the glob

## My solve
**Flag:** `pwn.college{UhxdFT9E3c0JsyULSo-v3shT-RK.QXzIDO0wiM5kjNzEzW}`

As mentioned, I channged the directory and then invoked the program while giving the argument `file_[absh]` so it would only find the desired files
```
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[absh]
You got it! Here is your flag!
pwn.college{UhxdFT9E3c0JsyULSo-v3shT-RK.QXzIDO0wiM5kjNzEzW}
```

## What I learned 
This question taught me about the glob `[]` and how it behaves as a single character wildcard but only for a specified set of characters, searching for patterns in names to complete the path

## Incorrect tangents 
N/A

## References 
N/A
