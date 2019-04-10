# Linux uptime Command
-------------------
### Command Introduction (命令介绍)
> **uptime - Tell how long the system has been running.**
### Command Format and Options (命令格式和选项)
```
#uptime --help

Usage:
 uptime [options]

Options:
 -p, --pretty   show uptime in pretty format
 -h, --help     display this help and exit
 -s, --since    system up since
 -V, --version  output version information and exit

For more details see uptime(1).
```
### Command Example (命令范例)
```

  uptime

  Tell how long the system has been running and other information.

  - Print current time, uptime, number of logged-in users and other information:
    uptime

  - Show only the amount of time the system has been booted for:
    uptime --pretty

  - Print the date and time the system booted up at:
    uptime --since

  - Show version information:
    uptime --version


```
