# Challenge 11 : Epic Filesystem Quest
This challenge will provide you with clues as to where the flag is and you need to follow it and use `ls`,`cd` and `cat` commands to find the flag using the clues and restrictions implemented

## My solve
**Flag:** `pwn.college{MXfCy8tg6kFwH0xK_xzW7Yw0JoR.QX5IDO0wiM5kjNzEzW}`

- Type in your solution and your thought process behind solving the challenge. 
- Include as much as info as possible. 
- Use triple ticks for bash.
- Try to explain in a step-by-step manner.
```
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.   .dockerenv  bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
..  NUGGET      boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~an-epic-filesystem-quest:/$ cat NUGGET
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/include/config/wlan
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/linux/linux-5.4/include/config/wlan
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/wlan$ ls -a
.  ..  CUE  vendor
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/wlan$ cat CUE
Great sleuthing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/werkzeug/datastructures/__pycache__

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/wlan$ cd /usr/local/lib/python3.8/dist-packages/werkzeug/datastructures/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/werkzeug/datastructures/__pycache__$ ls -a
.      __init__.cpython-38.pyc  cache_control.cpython-38.pyc  file_storage.cpython-38.pyc  range.cpython-38.pyc
..     accept.cpython-38.pyc    csp.cpython-38.pyc            headers.cpython-38.pyc       structures.cpython-38.pyc
.HINT  auth.cpython-38.pyc      etag.cpython-38.pyc           mixins.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/werkzeug/datastructures/__pycache__$ /.HINT
bash: /.HINT: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/werkzeug/datastructures/__pycache__$ cat .HINT
Congratulations, you found the clue!
The next clue is in: /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Size1

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/werkzeug/datastructures/__pycache__$ cd /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Size1
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Size1$ ls -a
.  ..  DOSSIER  Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Size1$ cat DOSSIER
Tubular find!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/feature/dd/signal

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Size1$ cd /opt/busybox/busybox-1.33.2/include/config/feature/dd/signal
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/dd/signal$ ls -a
.  ..  LEAD  handling.h
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/dd/signal$ cat LEAD
Tubular find!
The next clue is in: /usr/share/maxima-sage/5.42.2/share/vector

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/dd/signal$ ls -a /usr/share/maxima-sage/5.42.2/share/vector
.             rtest_vect.mac            vect.mac            vector.dem  vector_rebuild.lisp
..            rtest_vector_rebuild.mac  vect.usg            vector.mac  vector_rebuild.mac
MEMO-TRAPPED  vect.dem                  vect_transform.mac  vector.usg  vector_rebuild.usg
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/dd/signal$ cat /usr/share/maxima-sage/5.42.2/share/vector/MEMO-TRAPPED
Lucky listing!
The next clue is in: /usr/share/racket/pkgs/plot-doc/plot/scribblings/compiled

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/dd/signal$ cd /usr/share/racket/pkgs/plot-doc/plot/scribblings/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/plot-doc/plot/scribblings/compiled$ ls -a
.                 contracts_scrbl.dep    params_scrbl.zo     renderer2d_scrbl.dep    typed-compat_scrbl.zo
..                contracts_scrbl.zo     plot_scrbl.dep      renderer2d_scrbl.zo     utils_scrbl.dep
NOTE              intro_scrbl.dep        plot_scrbl.zo       renderer3d_scrbl.dep    utils_scrbl.zo
common_rkt.dep    intro_scrbl.zo         plotting_scrbl.dep  renderer3d_scrbl.zo
common_rkt.zo     nonrenderer_scrbl.dep  plotting_scrbl.zo   ticks_scrbl.dep
compat_scrbl.dep  nonrenderer_scrbl.zo   porting_scrbl.dep   ticks_scrbl.zo
compat_scrbl.zo   params_scrbl.dep       porting_scrbl.zo    typed-compat_scrbl.dep
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/plot-doc/plot/scribblings/compiled$ cat NOTE
Lucky listing!
The next clue is in: /usr/share/vim/vim81/lang/fi

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/plot-doc/plot/scribblings/compiled$ cd /usr/share/vim/vim81/lang/fi
hacker@commands~an-epic-filesystem-quest:/usr/share/vim/vim81/lang/fi$ ls -a
.  ..  LC_MESSAGES  MESSAGE
hacker@commands~an-epic-filesystem-quest:/usr/share/vim/vim81/lang/fi$ cat LC_MESSAGES
cat: LC_MESSAGES: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/share/vim/vim81/lang/fi$ cd LC_MESSAGES
hacker@commands~an-epic-filesystem-quest:/usr/share/vim/vim81/lang/fi/LC_MESSAGES$ ls -a
.  ..  vim.mo
hacker@commands~an-epic-filesystem-quest:/usr/share/vim/vim81/lang/fi/LC_MESSAGES$ cd /usr/share/vim/vim81/lang/fi
hacker@commands~an-epic-filesystem-quest:/usr/share/vim/vim81/lang/fi$ cat MESSAGE
Lucky listing!
The next clue is in: /usr/share/doc/libheimbase1-heimdal

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/vim/vim81/lang/fi$ cd /usr/share/doc/libheimbase1-heimdal
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libheimbase1-heimdal$ ls -a
.  ..  .CLUE  changelog.Debian.gz  copyright
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libheimbase1-heimdal$ cat .CLUE
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{MXfCy8tg6kFwH0xK_xzW7Yw0JoR.QX5IDO0wiM5kjNzEzW}
```

## What I learned 
I learnt how to better use the `ls`,`cd` commands to move through the directories, with certain restrictions

## Incorrect tangents 
N/A

## References 
N/A
