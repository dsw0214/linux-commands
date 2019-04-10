# Linux whoami Command
-------------------
### Command Introduction (命令介绍)
> **whoami - print effective userid**
### Command Format and Options (命令格式和选项)
```
#whoami --help
Usage: whoami [OPTION]...
Print the user name associated with the current effective user ID.
Same as id -un.

      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'whoami invocation'
```
### Command Example (命令范例)
```

  whoami

  Print the username associated with the current effective user ID.

  - Display currently logged username:
    whoami

  - Display the username after a change in the user ID:
    sudo whoami


```
