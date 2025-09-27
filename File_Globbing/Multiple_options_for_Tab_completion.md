# Challenge 9 : Multiple options for Tab completion
The challenge wants you to use tab completion when there are multiple possible matches

## My solve
**Flag:** `pwn.college{oSkazp-zWufoqd7njH6YeFqRCiC.0lN0EzNxwiM5kjNzEzW}`

As told in the challenge, I started by double clicking tab to see all the files starting with the name 'pwncollege-'
After this I `cat` the file with the flag in the using tab to put in the name faster
```
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-
pwncollege-family      pwncollege-flag        pwncollege-flamingo    pwncollege-flyswatter  pwncollege-hacking
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{oSkazp-zWufoqd7njH6YeFqRCiC.0lN0EzNxwiM5kjNzEzW}
```

## What I learned 
I learned that when there are multiple options while trying to use tab completion, double tapping tab will provide all possible matches, after which you can specify the tab completion further 

## Incorrect tangents 
N/A

## References 
N/A
