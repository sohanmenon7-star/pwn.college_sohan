# Challenge 5 : Searching for Manuals
This challenge instructs you to use `man man` to learn the advance uses of `man` using which to find the manpage in which the argument for the program is present in

## My solve
**Flag:** `pwn.college{0niTHYGNN2DMqYIde-E_98seuEm.QX2EDO0wiM5kjNzEzW}`

- As told in the challenge I inputted `man man` to learn about the `man` command
- After which I browsed through the details and found `man -k` which uses specified string as an argument and looks for any matches in all short manual pages
- After finding the manpage, I used the given argument as the argument for /challenge/challenge and found the flag
```
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -K flag
--Man-- next: etwdump(1) [ view (return) | skip (Ctrl-D) | quit (Ctrl-C) ]
^C
hacker@man~searching-for-manuals:~$ man -k flag
dpkg-buildflags (1)  - returns build flags to use during package build
Dpkg::BuildFlags (3perl) - query build flags
fegetexceptflag (3)  - floating-point rounding and exception handling
fesetexceptflag (3)  - floating-point rounding and exception handling
i386 (8)             - change reported architecture in new program environment and/or set personality flags
ioctl_iflags (2)     - ioctl() operations for inode flags
linux32 (1)          - change reported architecture in new program environment and/or set personality flags
linux64 (1)          - change reported architecture in new program environment and/or set personality flags
niqdeseumw (1)       - print the flag!
pcap-config (1)      - write libpcap compiler and linker flags to standard output
security_compute_av_flags (3) - query the SELinux policy database in the kernel
security_compute_av_flags_raw (3) - query the SELinux policy database in the kernel
set_matchpathcon_flags (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure ...
set_matchpathcon_invalidcon (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and confi...
set_matchpathcon_printf (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure...
setarch (1)          - change reported architecture in new program environment and/or set personality flags
setarch (8)          - change reported architecture in new program environment and/or set personality flags
x86_64 (8)           - change reported architecture in new program environment and/or set personality flags
hacker@man~searching-for-manuals:~$ man niqdeseumw
hacker@man~searching-for-manuals:~$ /challenge/challenge --niqdes 029
Correct usage! Your flag: pwn.college{0niTHYGNN2DMqYIde-E_98seuEm.QX2EDO0wiM5kjNzEzW}
```

## What I learned 
This challenge taught me about the advance properties of `man` andhow to access that data.
I also learnt that `man -k` can be used to find string in all short manuals with a match
(`man -K` for all manuals)

## Incorrect tangents 
While reading the manpage for `man`, I came across `-K` which is similar to `-k` except it searches all manpages available which is long, time-consuming and also brings up a lot of false positives and negatives

## References 
N/A
