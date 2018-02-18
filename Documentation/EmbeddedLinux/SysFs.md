# SysFs

> _sysfs is a pseudo file system provided by the Linux kernel that exports information about various kernel subsystems, hardware devices, and associated device drivers from the kernel's device model to user space through virtual files.[1] In addition to providing information about various devices and kernel subsystems, exported virtual files are also used for their configuring. sysfs provides functionality similar to the sysctl mechanism found in BSD operating systems, with the difference that sysfs is implemented as a virtual file system instead of being a purpose-built kernel mechanism, and that, in Linux, sysctl configuration parameters are made available at /proc/sys/ as part of procfs, not sysfs which is mounted at /sys/._ [Wikipedia](https://en.wikipedia.org/wiki/Sysfs)

```sh
pi@raspberrypi:~ $ mount | grep sysfs
sysfs on /sys type sysfs (rw,nosuid,nodev,noexec,relatime)
pi@raspberrypi:~ $ 
```