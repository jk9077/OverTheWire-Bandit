# Bandit Level 4 → Level 5

## Level goal

The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Commends used

file: determine file type

## Codes

```
ls
inhere
cd inhere
ls -al
total 48
drwxr-xr-x 2 root    root    4096 Jul 28 19:03 .
drwxr-xr-x 3 root    root    4096 Jul 28 19:03 ..
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file00
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file01
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file02
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file03
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file04
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file05
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file06
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file07
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file08
-rw-r----- 1 bandit5 bandit4   33 Jul 28 19:03 -file09
file ./*
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
cat ./-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQwc
