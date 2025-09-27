# Challenge 8 : Tab completion
The challenge asks you to hit tab in the shell to complete the path provided

## My solve
**Flag:** `pwn.college{ETpmUnWU7mEMboDJHJOYV4iGOTq.0FN0EzNxwiM5kjNzEzW}`

As explained in the challenge, I simply put the start of the path as the arguemnt to `cat` and finished up the path by htting 'tab'
```
hacker@globbing~tab-completion:~$ cat /challenge/pwncollege​
pwn.college{ETpmUnWU7mEMboDJHJOYV4iGOTq.0FN0EzNxwiM5kjNzEzW}
```

## What I learned 
I learnt that you can complete the path provided by hitting tab in the shell which is much more reliable than using the `*` which can give errors and saves a lot of time

## Incorrect tangents 
N/A

## References 
N/A
