# Challenge 8 : Foregrounding Processes
This challenge requires you to foreground a background process using `fg` so you can tinker with it and get the flag

## My solve
**Flag:** `pwn.college{E9Wf9rTPoFP0Ce3-WoDaO1c8nO_.QX4QDO0wiM5kjNzEzW}`

As told, I ran /challenge/run, suspended it using `Ctrl-Z`, backgrounded it using `bg` and then brought it back to the foreground of the terminal using `fg`
```
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~foregrounding-processes:~$


Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.

hacker@processes~foregrounding-processes:~$ fg
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{E9Wf9rTPoFP0Ce3-WoDaO1c8nO_.QX4QDO0wiM5kjNzEzW}
```

## What I learned 
I learned you can bring back processes running in the background using the `fg` command so you can mess with it a little more

## Incorrect tangents 
N/A

## References 
N/A
