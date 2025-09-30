# Challenge 3 : Multi-word Variables
This challenge is about assigning multi-word values to a variable

## My solve
**Flag:** `pwn.college{cIw0fcCKMIoUJvfMMls-IxMNW9Z.QXwYTN0wiM5kjNzEzW}`

As explained in the challenge, I set the value of PWN to "COLLEGE YEAH" using `=`
```
hacker@variables~multi-word-variables:~$ PWN="COLLEGE YEAH"
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{cIw0fcCKMIoUJvfMMls-IxMNW9Z.QXwYTN0wiM5kjNzEzW}
```

## What I learned 
- I learnt that you can assign multi-words values to variable by quoting the word with " "
- Spaces have a special meaning to the shell and thus multi words need to be quoted in order to be assigned

## Incorrect tangents 
N/A

## References 
N/A
