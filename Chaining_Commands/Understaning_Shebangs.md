# Challenge 7 : Understanding Shebangs
This challenge requires you to give a sheband to the script and then run a program to check if the shebag is in place

## My solve
**Flag:** `pwn.college{EoeaSrCi4OmFnScduEcwuVXBou3.0VOzMDOxwiM5kjNzEzW}`

- As told in teh challenge, I touched solve.sh and then gave it permission to execute
- After which i used `nano` to open the text editor and give the shebang `#!/bin/bash` as the first line followed by `echo "hack the planet"`
- Finally I ran the program /challenge/run to obtain the flag
```
hacker@chaining~understanding-shebangs:~$ touch solve.sh
hacker@chaining~understanding-shebangs:~$ nano solve.sh
hacker@chaining~understanding-shebangs:~$ cat solve.sh
#!/bin/bash

echo "hack the planet"
hacker@chaining~understanding-shebangs:~$ chmod ugo+x solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run
Testing your script...
Perfect! Your flag:
Flag: pwn.college{EoeaSrCi4OmFnScduEcwuVXBou3.0VOzMDOxwiM5kjNzEzW}
```

## What I learned 
- I leared about shebangs and how they are required for shell scripts, python scripts to run in the command shell
- I learned about `nano` which opens an inbuilt text editor of Linux, of the specified file to edit the contents

## Incorrect tangents 
- When I tried to `echo #!/bin/bash` it gave me an error Event not found 

## References 
Learnt about `nano` from a friend
