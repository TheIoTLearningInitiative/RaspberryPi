# Memory

> __Random-access memory (RAM /ræm/)__ _is a form of computer data storage that stores data and machine code currently being used. A random-access memory device allows data items to be read or written in almost the same amount of time irrespective of the physical location of data inside the memory._ [Wikipedia](https://en.wikipedia.org/wiki/Random-access_memory)

> __Paging__ _is a memory management scheme by which a computer stores and retrieves data from secondary storage[a] for use in main memory. In this scheme, the operating system retrieves data from secondary storage in same-size blocks called pages. Paging is an important part of virtual memory implementations in modern operating systems, using secondary storage to let programs exceed the size of available physical memory._ [Wikipedia](https://en.wikipedia.org/wiki/Paging)

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