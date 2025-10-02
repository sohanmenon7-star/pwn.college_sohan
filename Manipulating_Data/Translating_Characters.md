# Challenge 1 : Translating Characters
This challenge is about translating chracters from and specifically swap the cases for this question

## My solve
**Flag:** `pwn.college{4IPw7jYf6MN7l9B2JzV1F34RVp6.01MxEzNxwiM5kjNzEzW}`

Since this challenge asked you to swap the characters of the flag. To solve this I put the the inital arguemnt as all the alphabets and the second argument as what it the alphabets would be if they swap cases 
```
hacker@data~translating-characters:~$ /challenge/run | tr qwertyuiopasdfghjklzxcvbnmQWERTYUIOPASDFGHJKLZXCVBNM QWERTYUIOPASDFGHJKLZXCVBNMqwertyuiopasdfghjklzxcvbnm
yOUR CASE-SWAPPED FLAG:
pwn.college{4IPw7jYf6MN7l9B2JzV1F34RVp6.01MxEzNxwiM5kjNzEzW}
```

## What I learned 
- I learned about the `tr` command to change characters from the initial arguemnt to the characters in the final argument
- `tr` command takes stdin and prints out as stdout

## Incorrect tangents 
N/A

## References 
N/A
