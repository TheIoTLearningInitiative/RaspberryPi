# Memory

## Command free

```sh
FREE(1)                          User Commands                         FREE(1)

NAME
       free - Display amount of free and used memory in the system

SYNOPSIS
       free [options]

DESCRIPTION
       free  displays the total amount of free and used physical and swap mem‐
       ory in the system, as well as the buffers and caches used by  the  ker‐
       nel.  The  information  is  gathered by parsing /proc/meminfo. The dis‐
       played columns are:

       total  Total installed memory (MemTotal and SwapTotal in /proc/meminfo)
...
```

```sh
pi@raspberrypi:~ $ free
              total        used        free      shared  buff/cache   available
Mem:         949580      449408      225500       38592      274672      409512
Swap:        102396       17156       85240
pi@raspberrypi:~ $ free -m
              total        used        free      shared  buff/cache   available
Mem:            927         429         228          38         269         408
Swap:            99          16          83
pi@raspberrypi:~ $ 
```