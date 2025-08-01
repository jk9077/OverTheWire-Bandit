# Bandit Level 9 → Level 10

## Level goal

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## Commands used

strings: extract printable strings

## Codes
```
bandit9@bandit:~$ ls -al
total 40
drwxr-xr-x   2 root     root     4096 Jul 28 19:03 .
drwxr-xr-x 150 root     root     4096 Jul 28 19:06 ..
-rw-r--r--   1 root     root      220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root     3851 Jul 28 18:47 .bashrc
-rw-r-----   1 bandit10 bandit9 19379 Jul 28 19:03 data.txt
-rw-r--r--   1 root     root      807 Mar 31  2024 .profile
bandit9@bandit:~$ file ./data.txt
./data.txt: data
bandit9@bandit:~$ strings ./data.txt | grep =
Pw=h
========== the
C%m=
y7{1Z=
========== passwordb
#[q?=p
F========== is;o|
@[W=
p?e=	v
 K=r
V9V=]
U========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
u5=R
