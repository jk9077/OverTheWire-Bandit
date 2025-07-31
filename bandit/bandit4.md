# Bandit Level 3 → Level 4

## Level goal

The password for the next level is stored in a hidden file in the inhere directory.

## Commands used

cd: change the working directory

ls -al: list the all file in here

All . included in front of the filename are hidden file

## Codes
```
ls
inhere
cd inhere
ls -al
total 12
drwxr-xr-x 2 root    root    4096 Jul 28 19:03 .
drwxr-xr-x 3 root    root    4096 Jul 28 19:03 ..
-rw-r----- 1 bandit4 bandit3   33 Jul 28 19:03 ...Hiding-From-You
cat ...Hiding-From-You
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
