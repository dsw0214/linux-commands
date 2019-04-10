# Linux su Command
-------------------
### Command Introduction (命令介绍)
> **su - run a command with substitute user and group ID**
### Command Format and Options (命令格式和选项)
```
#su --help

Usage:
 su [options] [-] [USER [arg]...]

Change the effective user id and group id to that of USER.
A mere - implies -l.   If USER not given, assume root.

Options:
 -m, -p, --preserve-environment  do not reset environment variables
 -g, --group <group>             specify the primary group
 -G, --supp-group <group>        specify a supplemental group

 -, -l, --login                  make the shell a login shell
 -c, --command <command>         pass a single command to the shell with -c
 --session-command <command>     pass a single command to the shell with -c
                                 and do not create a new session
 -f, --fast                      pass -f to the shell (for csh or tcsh)
 -s, --shell <shell>             run shell if /etc/shells allows it

 -h, --help     display this help and exit
 -V, --version  output version information and exit

For more details see su(1).
```
### Command Example (命令范例)
```

  su

  Switch shell to another user.

  - Switch to superuser (admin password required):
    su

  - Switch to user {{username}} (password required):
    su username

  - Switch to user {{username}} and simulate a full login shell:
    su - username


```
