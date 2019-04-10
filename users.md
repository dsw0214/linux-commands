# Linux users Command
-------------------
### Command Introduction (命令介绍)
> **users - print the user names of users currently logged in to the current host**
### Command Format and Options (命令格式和选项)
```
#users --help
Usage: users [OPTION]... [FILE]
Output who is currently logged in according to FILE.
If FILE is not specified, use /var/run/utmp.  /var/log/wtmp as FILE is common.

      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'users invocation'
```
### Command Example (命令范例)
```

  users

  Display a list of logged in users.

  - Display a list of logged in users:
    users

  - Display a list of logged in users according to a specific file:
    users /var/log/wmtp


```
