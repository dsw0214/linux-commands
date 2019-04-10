# Linux iostat Command
-------------------
### Command Introduction (命令介绍)
> **iostat - Report Central Processing Unit (CPU) statistics and input/output statistics for devices and partitions.**
### Command Format and Options (命令格式和选项)
```
#iostat --help
# iostat --help
Usage: iostat [ options ] [ <interval> [ <count> ] ]
Options are:
[ -c ] [ -d ] [ -h ] [ -k | -m ] [ -N ] [ -t ] [ -V ] [ -x ] [ -y ] [ -z ]
[ -j { ID | LABEL | PATH | UUID | ... } ]
[ [ -T ] -g <group_name> ] [ -p [ <device> [,...] | ALL ] ]
[ <device> [...] | ALL ]
```
### Command Example (命令范例)
```

  iostat

  Report statistics for devices and partitions.

  - Display a report of CPU and disk statistics since system startup:
    iostat

  - Display a report of CPU and disk statistics with units converted to megabytes:
    iostat -m

  - Display CPU statistics:
    iostat -c

  - Display disk statistics with disk names (including LVM):
    iostat -N

  - Display extended disk statistics with disk names for device "sda":
    iostat -xN sda

  - Display incremental reports of CPU and disk statistics every 2 seconds:
    iostat 2

```
