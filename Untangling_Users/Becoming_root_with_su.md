# Challenge 1 : Becoming root with su
This challenge requires you to change the user to `root` using the `su` command, in which the flag is present

## My solve
**Flag:** `pwn.college{QfqsTwjPQYmHOXBveHKDqLf5Ax0.QX1UDN1wiM5kjNzEzW}`

- As told in the challenge, I changed the user to `root` using the `su` command and then providing the password given, hack-the-planet
- After which I simply used `cat /flag` to print the flag
```
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /challenge/flag
cat: /challenge/flag: No such file or directory
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{QfqsTwjPQYmHOXBveHKDqLf5Ax0.QX1UDN1wiM5kjNzEzW}
```

## What I learned 
This challenge taught me about users and how to change the user to `root` using the `su` command which means substitute user

## Incorrect tangents 
N/A

## References 
N/A
