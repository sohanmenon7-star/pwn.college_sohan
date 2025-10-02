# Challenge 4 : Extracting first few lines using head
The challenge tells you about the head command and how it can be used to pull the first few lines of its input
In this challenge, you have to pipe the first 7 lines of a program into another program

## My solve
**Flag:** `pwn.college{UvJEgSwppI-4mCcPRV64vtKA51A.0lNxEzNxwiM5kjNzEzW}`

- This question asks you to pipe the first 7 lines of /challenge/pwn into /challenge/college
- To do this, I piped /challenge/pwn into `head -n 7` command 
- I then piped this into /challenge/college using `|`
```
hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{UvJEgSwppI-4mCcPRV64vtKA51A.0lNxEzNxwiM5kjNzEzW}
```

## What I learned 
- I learned about the head command and how by default it will print out the first 10 lines of the stdin
- This can be controlled by using `-n` followed by the number of lines you want to print as stdout

## Incorrect tangents 
N/A

## References 
N/A

