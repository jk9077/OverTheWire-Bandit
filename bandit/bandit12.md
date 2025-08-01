# Bandit Level 11 → Level 12

## Level goal

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions


## Commands used

tr: translate characters

tr [ -cds ] [ string1 ] [ string2 ]: translate string1 to string 2

## Codes
bandit11@bandit:~$ ls -al
total 24
drwxr-xr-x   2 root     root     4096 Jul 28 19:03 .
drwxr-xr-x 150 root     root     4096 Jul 28 19:06 ..
-rw-r--r--   1 root     root      220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root     3851 Jul 28 18:47 .bashrc
-rw-r-----   1 bandit12 bandit11   49 Jul 28 19:03 data.txt
-rw-r--r--   1 root     root      807 Mar 31  2024 .profile
bandit11@bandit:~$ cat data.txt
Gur cnffjbeq vf 7k16JArUVv5LxVuJfsSVdbbtaHGlw9D4
bandit11@bandit:~$ cat ./data.txt | tr [A-Za-z] [N-ZA-Mn-za-m]
The password is 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
