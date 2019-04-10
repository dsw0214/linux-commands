# Linux fdisk Command
-------------------
### Command Introduction (命令介绍)
> **fdisk - manipulate disk partition table**
### Command Format and Options (命令格式和选项)
```
#fdisk --help
Usage:
 fdisk [options] <disk>    change partition table
 fdisk [options] -l <disk> list partition table(s)
 fdisk -s <partition>      give partition size(s) in blocks

Options:
 -b <size>             sector size (512, 1024, 2048 or 4096)
 -c[=<mode>]           compatible mode: 'dos' or 'nondos' (default)
 -h                    print this help text
 -u[=<unit>]           display units: 'cylinders' or 'sectors' (default)
 -v                    print program version
 -C <number>           specify the number of cylinders
 -H <number>           specify the number of heads
 -S <number>           specify the number of sectors per track
```
### Command Example (命令范例)
```

  fdisk

  A program for managing partition tables and partitions on a hard disk.

  - List partitions:
    fdisk -l

  - Start the partition manipulator:
    fdisk /dev/sda


```
