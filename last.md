# Linux last Command
-------------------
### Command Introduction (命令介绍)
> **last, lastb - show listing of last logged in users**
### Command Format and Options (命令格式和选项)
```
Usage: last [-num | -n num] [-f file] [-t YYYYMMDDHHMMSS] [-R] [-adioxFw] [username..] [tty..]
```
### Command Example (命令范例)
```

  last

  View the last logged in users.

  - View last logins, their duration and other information as read from /var/log/wtmp:
    last

  - Specify how many of the last logins to show:
    last -n login_count

  - Print the full date and time for entries and then display the hostname column last to prevent truncation:
    last -F -a

  - View all logins by a specific user and show the ip address instead of the hostname:
    last user_name -i

  - View all recorded reboots (i.e., the last logins of the pseudo user "reboot"):
    last reboot

  - View all recorded shutdowns (i.e., the last logins of the pseudo user "shutdown"):
    last shutdown


```
