# Bandit Level 5 → Level 6

## Level goal

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable

1033 bytes in size

not executable

## Commends used

find: search for files in a directory hierarchy

find [-H] [-L] [-P] [-D debugopts] [-Olevel] [starting-point...] [expression]

## Code
```
ls -al
total 88
drwxr-x--- 22 root bandit5 4096 Jul 28 19:03 .
drwxr-xr-x  3 root root    4096 Jul 28 19:03 ..
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere00
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere01
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere02
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere03
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere04
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere05
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere06
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere07
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere08
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere09
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere10
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere11
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere12
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere13
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere14
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere15
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere16
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere17
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere18
drwxr-x---  2 root bandit5 4096 Jul 28 19:03 maybehere19
fine -size 1033c
./maybehere07/.file2
cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
