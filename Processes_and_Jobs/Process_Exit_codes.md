# Challenge 10 : Process exit codes
This challenge asks you to exit a program and then read the exit code it produces and put that as the argument to the process you need to run to get the flag

## My solve
**Flag:** `pwn.college{s83ieGz1hOIAyJl2vtPJY5oQ1Hz.QX5YDO1wiM5kjNzEzW}`

- As told in the challenge, I ran /challenge/get-code which exited with a specific exit code
- To read this code, I used `echo $?`. This gave me the code
- I used this code as the argument to /challenge/submit-code to get the flag
```
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
65
hacker@processes~process-exit-codes:~$ /challenge/submit-code 65
CORRECT! Here is your flag:
pwn.college{s83ieGz1hOIAyJl2vtPJY5oQ1Hz.QX5YDO1wiM5kjNzEzW}
```

## What I learned 
- I learnt that each process, program, builtin exits with an exit code(`0` if it succeeded, random if it failed)
- More importantly I learnt how to read these exit codes using `?` prepended with `$`

## Incorrect tangents 
N/A

## References 
N/A
