# Challenge 6 : Mixing globs
This challenge asks you to use multiple globs together to match specified files

## My solve
**Flag:** `pwn.college{Y6Zx1yG0fj_actVG4fBknGwem27.QX1IDO0wiM5kjNzEzW}`

- In the challenge it was told that I needed to match the files 'challenging', 'educational' and 'pwning'.
- With this information, I first started with specifying a `[]` glob containing 'cep' as the start of the files begin with these letters.
- After which I added the `*` glob to complete the rest of the file name
```
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{Y6Zx1yG0fj_actVG4fBknGwem27.QX1IDO0wiM5kjNzEzW}
```

## What I learned 
I learnt in depth how to use multiple globs together to shorten an otherwise lengthy process of calling and searching for multiple files

## Incorrect tangents 
N/A

## References 
N/A
