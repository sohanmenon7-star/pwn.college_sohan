# Challenge 13 : Split piping stderr and stdout
This challenge asks you to send the stdout of a program into one command and the stderr of a program into another
using `>()`,`2>` and `|`
## My solve
**Flag:** `pwn.college{wp2kyjcQHw4oC0TeClbENi8UGm_.QXxQDM2wiM5kjNzEzW}`

- According to the challenge I needed to redirect the stdout into /challenge/planet and stderr into /challenge/the
- Since previously I have redirected stdout and stderr to seperate files, I used the same concept to solve this question
- Firstly I used `2> >()` to redirect stderr into /challenge/the` 
- Secondly I used `> >()` to redirect stdout into /challenge/planet. This gave me the flag
```
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the) > >(/challenge/planet)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{wp2kyjcQHw4oC0TeClbENi8UGm_.QXxQDM2wiM5kjNzEzW}
```

## What I learned 
- I learnt how to send stdout and stderr to seperate commands using `2>` and `>()`
- I learned more about process substitution specifically, `>()` and how it can take either stderr or stdout

## Incorrect tangents 
- I first tried to solve this by using `2>/challenge/the | /challenge/planet` but this did not work as it piped the stderr into /challenge/planet
- Second I tried `|/challenge/planet 2>/challenge/the` which did not work either because its was redirecting stdout into /challenge/the instead of stdout
- I also tried using `>(2>/challenge/the) | /challenge/planet`. This failed and i learned that `>()` can only either take stdout at a time or stderr

## References 
N/A
