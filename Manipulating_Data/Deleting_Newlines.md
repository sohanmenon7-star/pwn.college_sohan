# Challenge 3 : Deleting newlines
This challenge teaches about newlines and in this challenge you have to delete all the newlines("\n")

## My solve
**Flag:** `pwn.college{saq7nxHvLR-IYxkz6tvqGhtgjkI.0VNxEzNxwiM5kjNzEzW}`

- This challegne asks you to delete all new lines using `tr -d`
- To do this I simply put "\n" as the arguemt to the command `tr -d` to delete them and give a single line output
```
hacker@data~deleting-newlines:~$ /challenge/run | tr -d "\n"
Your line-split flag: pwn.college{saq7nxHvLR-IYxkz6tvqGhtgjkI.0VNxEzNxwiM5kjNzEzW}
```

## What I learned 
- I learned about newline "\n" and how it is used to change lines by the shell and how it can be used with `tr` to replace characters or even get deleted
- \n needs to be in quotes so the shell doesnt interpret it and pass it to `tr`

## Incorrect tangents 
N/A

## References 
N/A
