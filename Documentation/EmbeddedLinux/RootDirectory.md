# Root Directory

From Linux Documentation Project [Chapter 1. Linux Filesystem Hierarchy](http://www.tldp.org/LDP/Linux-Filesystem-Hierarchy/html/the-root-directory.html)

```
To comply with the FSSTND the following directories, or symbolic links to directories, are required in /.

       /bin       Essential command binaries
       /boot      Static files of the boot loader
       /dev       Device files
       /etc       Host-specific system configuration
       /lib       Essential shared libraries and kernel modules
       /media     Mount point for removeable media
       /mnt       Mount point for mounting a filesystem temporarily
       /opt       Add-on application software packages
       /sbin      Essential system binaries
       /srv       Data for services provided by this system
       /tmp       Temporary files
       /usr       Secondary hierarchy
       /var       Variable data
       
The following directories, or symbolic links to directories, must be in /, if the corresponding subsystem is installed:

     / -- the root directory
     /home User home directories (optional)
     /lib<qual> Alternate format essential shared libraries
                      (optional)
     /root Home directory for the root user (optional)
```

```sh
pi@raspberrypi:~ $ cd /
pi@raspberrypi:/ $ tree -L 1
.
├── bin
├── boot
├── dev
├── etc
├── home
├── lib
├── lost+found
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin
├── srv
├── sys
├── tmp
├── usr
└── var

19 directories, 0 files
pi@raspberrypi:/ $ cd
pi@raspberrypi:~ $ 
```