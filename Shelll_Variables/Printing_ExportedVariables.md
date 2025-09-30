# Challenge 5 : Printing Exported Variables
The challenge wants you to use the `env` command to print all exported variables one of which being FLAG

## My solve
**Flag:** `pwn.college{EJFE7PPo5_D8U5dxqHytYuzfXki.QX4UTN0wiM5kjNzEzW}`

As instructed in the challenge, I simply exported FLAG and then ran the `env` command to obtain the flag
```
hacker@variables~printing-exported-variables:~$ export FLAG
hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=bc1ea17d779d086c531c8a402afb469c8246661c3a1a5549dc1a0a863827fe8d
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{EJFE7PPo5_D8U5dxqHytYuzfXki.QX4UTN0wiM5kjNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

## What I learned 
I learnt another method to print variables, specifically all exported variables

## Incorrect tangents 
N/A

## References 
N/A
