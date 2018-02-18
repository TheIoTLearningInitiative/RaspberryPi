# Debug Filesystem

> _debugfs is a special file system available in the Linux kernel since version 2.6.10-rc3. It was written by Greg Kroah-Hartman. debugfs is a simple-to-use RAM-based file system specially designed for debugging purposes. It exists as a simple way for kernel developers to make information available to user space. Unlike /proc, which is only meant for information about a process, or sysfs, which has strict one-value-per-file rules, debugfs has no rules at all. Developers can put any information they want there. [Wikipedia](https://en.wikipedia.org/wiki/Debugfs)

```sh
pi@raspberrypi:~ $ mount | grep  debugfs
debugfs on /sys/kernel/debug type debugfs (rw,relatime)
pi@raspberrypi:~ $ 
```