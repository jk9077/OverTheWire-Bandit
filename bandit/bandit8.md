# Bandit Level 7 → Level 8

## Level goal

The password for the next level is stored in the file data.txt next to the word millionth

## Commends used

grep:  searching  for  PATTERNS  in  each  FILE

## Codes
```
bandit7@bandit:~$ ls -al
total 4108
drwxr-xr-x   2 root    root       4096 Jul 28 19:04 .
drwxr-xr-x 150 root    root       4096 Jul 28 19:06 ..
-rw-r--r--   1 root    root        220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root    root       3851 Jul 28 18:47 .bashrc
-rw-r-----   1 bandit8 bandit7 4184396 Jul 28 19:04 data.txt
-rw-r--r--   1 root    root        807 Mar 31  2024 .profile
bandit7@bandit:~$ grep millionth ./data.txt
millionth	dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
