# Linux w Command
-------------------
### Command Introduction (命令介绍)
> **w - Show who is logged on and what they are doing.**
### Command Format and Options (命令格式和选项)
```
# w --help

Usage:
 w [options]

Options:
 -h, --no-header     do not print header
 -u, --no-current    ignore current process username
 -s, --short         short format
 -f, --from          show remote hostname field
 -o, --old-style     old style output
 -i, --ip-addr       display IP address instead of hostname (if possible)

     --help     display this help and exit
 -V, --version  output version information and exit

For more details see w(1).
```
### Command Example (命令范例)
```
  w

  Show who is logged on and what they are doing.
  Print user login, TTY, remote host, login time, idle time, current process.

  - Show logged-in users info:
    w

  - Show logged-in users info without a header:
    w -h
```
