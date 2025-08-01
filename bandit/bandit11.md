# Bandit Level 10 → Level 11

## Level goal

The password for the next level is stored in the file data.txt, which contains base64 encoded data

## Commands used

~==: encoding to base64

base64: encode/decode data and print to standard output

base64 [option] [file]

-d: decode

-i: ignore non-alphabet characters

-w: wrap encoded lines after cols characters

## Codes
```
bandit10@bandit:~$ ls -al
total 24
drwxr-xr-x   2 root     root     4096 Jul 28 19:03 .
drwxr-xr-x 150 root     root     4096 Jul 28 19:06 ..
-rw-r--r--   1 root     root      220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root     3851 Jul 28 18:47 .bashrc
-rw-r-----   1 bandit11 bandit10   69 Jul 28 19:03 data.txt
-rw-r--r--   1 root     root      807 Mar 31  2024 .profile
bandit10@bandit:~$ base64 -d data.txt
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
