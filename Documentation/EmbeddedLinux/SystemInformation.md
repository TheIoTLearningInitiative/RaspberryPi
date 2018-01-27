# System Information

```sh
UNAME(1)                         User Commands                        UNAME(1)

NAME
       uname - print system information

SYNOPSIS
       uname [OPTION]...

DESCRIPTION
       Print certain system information.  With no OPTION, same as -s.

       -a, --all
              print  all  information,  in the following order, except omit -p
              and -i if unknown:
...
```

```sh
pi@raspberrypi:~ $ uname -a
Linux raspberrypi 4.9.59-v7+ #1047 SMP Sun Oct 29 12:19:23 GMT 2017 armv7l GNU/Linux
pi@raspberrypi:~ $ 
```