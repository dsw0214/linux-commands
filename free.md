# Linux free Command
### Command Introduction (命令介绍)
-------------------
> **free - Display amount of free and used memory in the system**
### Command Format and Options (命令格式和选项)
```
#free --help

Usage:
 free [options]

Options:
 -b, --bytes         show output in bytes
 -k, --kilo          show output in kilobytes
 -m, --mega          show output in megabytes
 -g, --giga          show output in gigabytes
     --tera          show output in terabytes
 -h, --human         show human-readable output
     --si            use powers of 1000 not 1024
 -l, --lohi          show detailed low and high memory statistics
 -t, --total         show total for RAM + swap
 -s N, --seconds N   repeat printing every N seconds
 -c N, --count N     repeat printing N times, then exit
 -w, --wide          wide output

     --help     display this help and exit
 -V, --version  output version information and exit

For more details see free(1).
```
### Command Example (命令范例)
-------------------
**Display amount of free and used memory in the system.**

- Display system memory:

  ` free`

- Display memory in Bytes/KB/MB/GB:

  ` free -b|k|m|g`

- Display memory in human readable units:

  ` free -h`

- Refresh the output every 2 seconds:

  ` free -s 2`
