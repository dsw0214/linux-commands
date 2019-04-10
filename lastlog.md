# Linux lastof Command
-------------------
### Command Introduction (命令介绍)
> **lastlog - reports the most recent login of all users or of a given user**
### Command Format and Options (命令格式和选项)
```
# lastlog --help
Usage: lastlog [options]

Options:
  -b, --before DAYS             print only lastlog records older than DAYS
  -C, --clear                   clear lastlog record of an user (usable only with -u)
  -h, --help                    display this help message and exit
  -R, --root CHROOT_DIR         directory to chroot into
  -S, --set                     set lastlog record to current time (usable only with -u)
  -t, --time DAYS               print only lastlog records more recent than DAYS
  -u, --user LOGIN              print lastlog record of the specified LOGIN
```
### Command Example (命令范例)
```
  lastlog

    Show the most recent login of all users or of a given user.

    - Display the most recent login of all users:
      lastlog

    - Display lastlog record of the specified user:
      lastlog -u username

    - Display records before than 7 days:
      lastlog -b 7

    - Display records more recent than 3 days:
      lastlog -t 3
```
