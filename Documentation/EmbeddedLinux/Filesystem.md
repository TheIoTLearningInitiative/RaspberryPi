# Filesystem

> In computing, a file system (or filesystem) is used to control how data is stored and retrieved. Without a file system, information placed in a storage area would be one large body of data with no way to tell where one piece of information stops and the next begins. By separating the data into pieces and giving each piece a name, the information is easily isolated and identified. Taking its name from the way paper-based information systems are named, each group of data is called a "file". The structure and logic rules used to manage the groups of information and their names is called a "file system". [Wikipedia](https://en.wikipedia.org/wiki/File_system)

## Command df

```sh
DF(1)                            User Commands                           DF(1)

NAME
       df - report file system disk space usage

SYNOPSIS
       df [OPTION]... [FILE]...

DESCRIPTION
       This  manual  page  documents  the  GNU version of df.  df displays the
       amount of disk space available on the file system containing each  file
       name  argument.   If  no file name is given, the space available on all
       currently mounted file systems is shown.  Disk space  is  shown  in  1K
       blocks  by  default, unless the environment variable POSIXLY_CORRECT is
       set, in which case 512-byte blocks are used.
...
```

```sh
pi@raspberrypi:~ $ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/root       7.1G  4.2G  2.6G  62% /
devtmpfs        460M     0  460M   0% /dev
tmpfs           464M   29M  435M   7% /dev/shm
tmpfs           464M   18M  446M   4% /run
tmpfs           5.0M  4.0K  5.0M   1% /run/lock
tmpfs           464M     0  464M   0% /sys/fs/cgroup
/dev/mmcblk0p1   41M   21M   21M  51% /boot
tmpfs            93M     0   93M   0% /run/user/1000
pi@raspberrypi:~ $ 
```