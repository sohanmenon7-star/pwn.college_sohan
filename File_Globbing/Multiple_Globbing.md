# Challenge 5 : Multiple globbing
This challenge is about teaching the use of multiple globs at the same time, asking you to use `*` twice

## My solve
**Flag:** `pwn.college{AfboWJrajEQy2twyMpN2GnXopRA.0lM3kjNxwiM5kjNzEzW}`

As instructed in the challenge, I changed directories and then ran the program with a single argument `*p*` as specified in the question
```
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{AfboWJrajEQy2twyMpN2GnXopRA.0lM3kjNxwiM5kjNzEzW}
```

## What I learned 
- I learnt that you can use multiple globs at the same time to reduce the time spent typing when the file names are large and complex
- Using `*` before a specification will bring all file matches including nothing before the specified value
- Using `*` after a specification will bring all file matches including nothing after the specified value

## Incorrect tangents 
N/A

## References 
N/A
