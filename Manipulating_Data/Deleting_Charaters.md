# Challenge 2 : Deleting Characters
This challenge is about deleting '%^' from the flag using `tr -d`

## My solve
**Flag:** `pwn.college{oyVQUJLS9QgqmEmXGNjhJhGC2dP.0FNxEzNxwiM5kjNzEzW}`

- This challenge tells me to use `tr -d` to translate characters to nothing(deleting them)
- As asked in the challenge I put '%^' as the arguemnt to `tr -d` command to delete them from the flag to obtain the correct value
```
hacker@data~deleting-characters:~$ /challenge/run | tr -d ^%
Your character-stuffed flag:
pwn.college{oyVQUJLS9QgqmEmXGNjhJhGC2dP.0FNxEzNxwiM5kjNzEzW}
```

## What I learned 
I learnt that you can delete characters from a file using `tr -d` by putting the characters you want to delete as the argument

## Incorrect tangents 
N/A

## References 
N/A
