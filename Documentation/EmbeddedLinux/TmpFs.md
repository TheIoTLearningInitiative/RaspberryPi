# TmpFs

> _tmpfs is a common name for a temporary file storage facility on many Unix-like operating systems. It is intended to appear as a mounted file system, but stored in volatile memory instead of a persistent storage device. A similar construction is a RAM disk, which appears as a virtual disk drive and hosts a disk file system._ [Wikipedia](https://en.wikipedia.org/wiki/Tmpfs)

```sh
pi@raspberrypi:~ $ mount | grep tmpfs
devtmpfs on /dev type devtmpfs (rw,relatime,size=470180k,nr_inodes=117545,mode=755)
tmpfs on /dev/shm type tmpfs (rw,nosuid,nodev)
tmpfs on /run type tmpfs (rw,nosuid,nodev,mode=755)
tmpfs on /run/lock type tmpfs (rw,nosuid,nodev,noexec,relatime,size=5120k)
tmpfs on /sys/fs/cgroup type tmpfs (ro,nosuid,nodev,noexec,mode=755)
tmpfs on /run/user/1000 type tmpfs (rw,nosuid,nodev,relatime,size=94956k,mode=700,uid=1000,gid=1000)
pi@raspberrypi:~ $ 
```