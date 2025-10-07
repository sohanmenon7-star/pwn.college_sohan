# Challenge 3 : Handling Failure
In this challenge you have to use `||` to chain two commands to get the flag

## My solve
**Flag:** `pwn.college{kHWxhfuqkQ3qht0GuOVCEYbPoGE.01M0MDOxwiM5kjNzEzW}`

As told in the challenge, I simply used `||` to chain /challenge/first-failure and /challenge/second to get the flag
```
hacker@chaining~handling-failure:~$ /challenge/first-failure || /challenge/second
Nice chaining! Flag: pwn.college{kHWxhfuqkQ3qht0GuOVCEYbPoGE.01M0MDOxwiM5kjNzEzW}
```

## What I learned 
This challenge taught me how to use `||` which chains only IF the first command fails

## Incorrect tangents 
N/A

## References 
N/A
