# Linux id Command
-------------------
### Command Introduction (命令介绍)
> **id - print real and effective user and group IDs**
### Command Format and Options (命令格式和选项)
```
#id --help
Usage: id [OPTION]... [USER]
Print user and group information for the specified USER,
or (when USER omitted) for the current user.

  -a             ignore, for compatibility with other versions
  -Z, --context  print only the security context of the current user
  -g, --group    print only the effective group ID
  -G, --groups   print all group IDs
  -n, --name     print a name instead of a number, for -ugG
  -r, --real     print the real ID instead of the effective ID, with -ugG
  -u, --user     print only the effective user ID
  -z, --zero     delimit entries with NUL characters, not whitespace;
                   not permitted in default format
      --help     display this help and exit
      --version  output version information and exit

Without any OPTION, print some useful set of identified information.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'id invocation'
```
### Command Example (命令范例)
```

  id

  Display current user and group identity.

  - Display current user's id (UID), group id (GID) and groups to which they belong:
    id

  - Display the current user identity as a number:
    id -u

  - Display the current group identity as a number:
    id -g

  - Display an arbitrary user's id (UID), group id (GID) and groups to which they belong:
    id username


```
