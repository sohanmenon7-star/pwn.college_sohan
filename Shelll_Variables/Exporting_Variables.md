# Challenge 4 : Exporting Variables
The challenge asks you to export the vairables to the child shell and then invoke a program with the variable

## My solve
**Flag:** `pwn.college{oPS2sg9_ZJQB7l3IQwYYVoiDDOM.QXyYTN0wiM5kjNzEzW}`

- As instructed in the program, I exported PWN and set its value to COLLEGE
- I did NOT export COLLEGE but assigned the value of PWN to it
- Finally, I invoked the program to finish the challenge
```
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run $PWN $COLLEGE
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{oPS2sg9_ZJQB7l3IQwYYVoiDDOM.QXyYTN0wiM5kjNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```

## What I learned 
I learnt that the variables need to the exported to the child shell `sh`/`$` to be used in programs and commands
Once, the child shell recieves the variable, it can be used

## Incorrect tangents 
N/A

## References 
N/A
