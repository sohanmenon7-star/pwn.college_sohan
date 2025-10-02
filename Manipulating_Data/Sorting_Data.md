# Challenge 6 : Sorting Data
This challenge teaches you about sorting data using `sort` and has the correct flag as the 100th element of the sorted file

## My solve
**Flag:** `pwn.college{02IjWj4U9RHY6x_PjppEfdvRybl.0FM0MDOxwiM5kjNzEzW}`

To complete this challenge, I simply used teh `sort -r` command to order the lines in a reverse alphabetical order so the correct flag would be at the top 
```
hacker@data~sorting-data:~$ sort -r /challenge/flags.txt
pwn.college{02IjWj4U9RHY6x_PjppEfdvRybl.0FM0MDOxwiM5kjNzEzW}
pwn.college{02IjWj4U9RHY6x_PjppEfdvRybl.0FM0MDOxwiM5kjNzDzW}
pwn.college{02IjWj4U9RHY6x_PjppEfdvRybl.0FM0MDOxwiM5kjNyEzW}
pwn.college{02IjWj4U9RHY6x_PjopEfdvRyal.0FM0MCOxwiL5kjNzEzW}
pwn.college{02IjWj4U9RHX6x_PjpoEfcvRxal.0FM0LDNxviL5jiNzEzW}
. . .
```

## What I learned 
- I learned how to sort lines of data using `sort` and how it can be valueable for large files
- `sort` command has arguments to control the order of sorting, `-r` : Reverse, `-u` : Uniques, `-R` : Random

## Incorrect tangents 
N/A

## References 
N/A
