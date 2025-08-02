# Bandit Level 13 → Level 14

## Level goal

The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

## Commands used

ssh -i [file]: using file as a password

## Codes
```
bandit13@bandit:~$ ls -al
total 24
drwxr-xr-x   2 root     root     4096 Jul 28 19:03 .
drwxr-xr-x 150 root     root     4096 Jul 28 19:06 ..
-rw-r--r--   1 root     root      220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root     root     3851 Jul 28 18:47 .bashrc
-rw-r--r--   1 root     root      807 Mar 31  2024 .profile
-rw-r-----   1 bandit14 bandit13 1679 Jul 28 19:03 sshkey.private
bandit13@bandit:~$ file ./sshkey.private
./sshkey.private: PEM RSA private key
bandit13@bandit:~$ ssh -i ./sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
