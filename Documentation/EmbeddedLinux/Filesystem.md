# Filesystem

> In computing, a file system (or filesystem) is used to control how data is stored and retrieved. Without a file system, information placed in a storage area would be one large body of data with no way to tell where one piece of information stops and the next begins. By separating the data into pieces and giving each piece a name, the information is easily isolated and identified. Taking its name from the way paper-based information systems are named, each group of data is called a "file". The structure and logic rules used to manage the groups of information and their names is called a "file system". [Wikipedia](https://en.wikipedia.org/wiki/File_system)

## Command fs

```sh
FILESYSTEMS(5)             Linux Programmer's Manual            FILESYSTEMS(5)

NAME
       filesystems  -  Linux  filesystem  types:  ext, ext2, ext3, ext4, hpfs,
       iso9660, JFS, minix, msdos, ncpfs nfs, ntfs, proc, Reiserfs, smb, sysv,
       umsdos, vfat, XFS, xiafs,

DESCRIPTION
       When, as is customary, the proc filesystem is mounted on /proc, you can
       find in  the  file  /proc/filesystems  which  filesystems  your  kernel
       currently  supports;  see  proc(5)  for  more  details.   If you need a
       currently unsupported filesystem, insert the  corresponding  module  or
       recompile the kernel.
...
```