# Bandit Level 6 → Level 7

## Level goal

The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7

owned by group bandit6

33 bytes in size

## Commends used

find -user username -group groupname
2>/dev/null: move error data into the Trash

## Codes
```
bandit6@bandit:~$ ls -al
total 20
drwxr-xr-x   2 root root 4096 Jul 28 19:03 .
drwxr-xr-x 150 root root 4096 Jul 28 19:06 ..
-rw-r--r--   1 root root  220 Mar 31  2024 .bash_logout
-rw-r--r--   1 root root 3851 Jul 28 18:47 .bashrc
-rw-r--r--   1 root root  807 Mar 31  2024 .profile
bandit6@bandit:~$ find /-size 33c -user bandit7 -group bandit6
find: ‘/sys/kernel/tracing’: Permission denied
find: ‘/sys/kernel/debug’: Permission denied
find: ‘/sys/fs/pstore’: Permission denied
find: ‘/sys/fs/bpf’: Permission denied
find: ‘/tmp’: Permission denied
find: ‘/run/udisks2’: Permission denied
find: ‘/run/chrony’: Permission denied
find: ‘/run/user/11026’: Permission denied
find: ‘/run/user/11003’: Permission denied
find: ‘/run/user/11011’: Permission denied
find: ‘/run/user/11010’: Permission denied
find: ‘/run/user/11014’: Permission denied
find: ‘/run/user/11015’: Permission denied
find: ‘/run/user/12001’: Permission denied
find: ‘/run/user/12002’: Permission denied
find: ‘/run/user/11024’: Permission denied
find: ‘/run/user/11031’: Permission denied
find: ‘/run/user/11017’: Permission denied
find: ‘/run/user/11025’: Permission denied
find: ‘/run/user/11021’: Permission denied
find: ‘/run/user/11023’: Permission denied
find: ‘/run/user/11009’: Permission denied
find: ‘/run/user/11013’: Permission denied
find: ‘/run/user/11000’: Permission denied
find: ‘/run/user/11022’: Permission denied
find: ‘/run/user/0’: Permission denied
find: ‘/run/user/11008’: Permission denied
find: ‘/run/user/11007’: Permission denied
find: ‘/run/user/11012’: Permission denied
find: ‘/run/user/11001’: Permission denied
find: ‘/run/user/11006/systemd/inaccessible/dir’: Permission denied
find: ‘/run/user/11005’: Permission denied
find: ‘/run/user/11004’: Permission denied
find: ‘/run/user/11016’: Permission denied
find: ‘/run/user/11002’: Permission denied
find: ‘/run/sudo’: Permission denied
find: ‘/run/screen/S-bandit20’: Permission denied
find: ‘/run/multipath’: Permission denied
find: ‘/run/cryptsetup’: Permission denied
find: ‘/run/lvm’: Permission denied
find: ‘/run/systemd/propagate/fwupd.service’: Permission denied
find: ‘/run/systemd/propagate/ModemManager.service’: Permission denied
find: ‘/run/systemd/propagate/polkit.service’: Permission denied
find: ‘/run/systemd/propagate/chrony.service’: Permission denied
find: ‘/run/systemd/propagate/systemd-logind.service’: Permission denied
find: ‘/run/systemd/propagate/irqbalance.service’: Permission denied
find: ‘/run/systemd/propagate/systemd-networkd.service’: Permission denied
find: ‘/run/systemd/propagate/systemd-resolved.service’: Permission denied
find: ‘/run/systemd/propagate/systemd-udevd.service’: Permission denied
find: ‘/run/systemd/inaccessible/dir’: Permission denied
find: ‘/run/lock/lvm’: Permission denied
find: ‘/boot/lost+found’: Permission denied
find: ‘/boot/efi’: Permission denied
find: ‘/lost+found’: Permission denied
find: ‘/dev/mqueue’: Permission denied
find: ‘/dev/shm’: Permission denied
find: ‘/root’: Permission denied
find: ‘/var/spool/bandit24’: Permission denied
find: ‘/var/spool/cron/crontabs’: Permission denied
find: ‘/var/spool/rsyslog’: Permission denied
find: ‘/var/tmp’: Permission denied
find: ‘/var/crash’: Permission denied
find: ‘/var/cache/private’: Permission denied
find: ‘/var/cache/pollinate’: Permission denied
find: ‘/var/cache/ldconfig’: Permission denied
find: ‘/var/cache/apt/archives/partial’: Permission denied
find: ‘/var/cache/apparmor/ac99afeb.0’: Permission denied
find: ‘/var/cache/apparmor/2693c843.0’: Permission denied
find: ‘/var/log’: Permission denied
find: ‘/var/lib/update-notifier/package-data-downloads/partial’: Permission denied
find: ‘/var/lib/chrony’: Permission denied
find: ‘/var/lib/private’: Permission denied
/var/lib/dpkg/info/bandit7.password
find: ‘/var/lib/polkit-1’: Permission denied
find: ‘/var/lib/snapd/cookie’: Permission denied
find: ‘/var/lib/snapd/void’: Permission denied
find: ‘/var/lib/amazon’: Permission denied
find: ‘/var/lib/udisks2’: Permission denied
find: ‘/var/lib/apt/lists/partial’: Permission denied
find: ‘/var/lib/fwupd/gnupg’: Permission denied
find: ‘/var/lib/ubuntu-advantage/apt-esm/var/lib/apt/lists/partial’: Permission denied
find: ‘/snap’: Permission denied
find: ‘/proc/tty/driver’: Permission denied
find: ‘/proc/2884815/task/2884815/fd/6’: No such file or directory
find: ‘/proc/2884815/task/2884815/fdinfo/6’: No such file or directory
find: ‘/proc/2884815/fd/5’: No such file or directory
find: ‘/proc/2884815/fdinfo/5’: No such file or directory
find: ‘/manpage/manpage3-pw’: Permission denied
find: ‘/etc/stunnel’: Permission denied
find: ‘/etc/polkit-1/rules.d’: Permission denied
find: ‘/etc/credstore.encrypted’: Permission denied
find: ‘/etc/multipath’: Permission denied
find: ‘/etc/sudoers.d’: Permission denied
find: ‘/etc/xinetd.d’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
find: ‘/etc/credstore’: Permission denied
find: ‘/drifter/drifter14_src/axTLS’: Permission denied
find: ‘/home/leviathan0/.backup’: Permission denied
find: ‘/home/drifter8/chroot’: Permission denied
find: ‘/home/bandit29-git’: Permission denied
find: ‘/home/bandit28-git’: Permission denied
find: ‘/home/leviathan4/.trash’: Permission denied
find: ‘/home/ubuntu’: Permission denied
find: ‘/home/drifter6/data’: Permission denied
find: ‘/home/bandit30-git’: Permission denied
find: ‘/home/bandit27-git’: Permission denied
find: ‘/home/bandit5/inhere’: Permission denied
find: ‘/home/bandit31-git’: Permission denied
bandit6@bandit:~$ find / -size 33c -user bandit7 -group bandit6 2> /dev/null
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
