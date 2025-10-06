# Challenge 5 : Executing Files 
In this challenge instead of reading the file after giving permission you have execute a program after giving permission in a similar way as the last challenge

## My solve
**Flag:** `pwn.college{QK-Xu6e0vjiKrcE_oLECPgeJ5_3.QXyEjN0wiM5kjNzEzW}`

As explained in the challenge, I used `chmod` to give permission to the user owner to execute the program, thus giving me the answer
```
hacker@permissions~executable-files:~$ chmod u+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{QK-Xu6e0vjiKrcE_oLECPgeJ5_3.QXyEjN0wiM5kjNzEzW}
```

## What I learned 
I learned about using `chmod` to give permission to users, groups, owners to execute a program

## Incorrect tangents 
N/A

## References 
N/A
