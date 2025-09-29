# Challenge 9 : Filtering with grep -v
This challenge is about using `grep -v` to eliminate all undesirable lines and thus filter out the required flag

## My solve
**Flag:** `pwn.college{AoZOtp7VG3s7EWHVbmzbSwVpzNK.0FOxEzNxwiM5kjNzEzW}`

As told in the challenge, I simply used the `|` to redirect the standard output to the command `grep -v`
In the command `grep -v` I gave DECOY as the argument as it was told in the challenge to the incorrect files have the word DECOY in them 
```
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{AoZOtp7VG3s7EWHVbmzbSwVpzNK.0FOxEzNxwiM5kjNzEzW}
```

## What I learned 
I learned about the invert match of the `grep` command and how it can be used to filter out all unwanted lines by giving a string in its argument it will NOT show the line matches

## Incorrect tangents 
N/A

## References 
N/A
