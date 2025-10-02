# Challenge 5 : Extracting specific sections
In this challenge you have to use the `cut` command to extraxt a specific coloumn and then delete the newlines to change the coloumn to a line 

## My solve
**Flag:** `pwn.college{gGcGd_zJUS37D7mmMWumz3YzOWU.01NxEzNxwiM5kjNzEzW}`

- To solve this challenge, I first saw which column had the flag characters
- Once I found it, I used the `cut -d " " -f 2` to extract column 2 pipe it into `tr -d "\n"` deleting the newlines and obtaining the flag 
```
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run
25810 p
8713 w
5183 n
16307 .
9485 c
9033 o
5456 l
24901 l
5579 e
32149 g
95 e
4197 {
27646 g
654 G
15005 c
6769 G
32450 d
29858 _
29546 z
23662 J
27866 U
5994 S
15086 3
28862 7
27851 D
5095 7
19595 m
26656 m
14902 M
21644 W
18649 u
21893 m
12524 z
26520 3
11383 Y
26403 z
23689 O
26032 W
3733 U
26043 .
2010 0
8317 1
5538 N
18985 x
23383 E
15799 z
31209 N
23447 x
7725 w
13448 i
29540 M
11098 5
24551 k
14617 j
13823 N
9057 z
19795 E
9747 z
19407 W
6038 }
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{gGcGd_zJUS37D7mmMWumz3YzOWU.01NxEzNxwiM5kjNzEzW}
```

## What I learned 
- I learned about the command `cut` command which can be used to extract a selected column
- `-d` is the column delimiter which is what seperates the column 
- `-f` is the field number(The column number to be extracted)

## Incorrect tangents 
N/A

## References 
N/A
