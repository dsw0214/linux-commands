# Linux ps Command
### Command Introduction (命令介绍)
-------------------
> ** ps - report a snapshot of the current processes. **

### Command Format and Options (命令格式和选项)
```
#ps --help

Usage:
 ps [options]

 Try 'ps --help <simple|list|output|threads|misc|all>'
  or 'ps --help <s|l|o|t|m|a>'
 for additional help text.

For more details see ps(1).
```
### Command Example (命令范例)
-------------------
** Information about running processes. **

- List all running processes:

  ` ps aux`

- List all running processes including the full command string:

  ` ps auxww`

- Search for a process that matches a string:

  ` ps aux | grep string`

- List all processes of the current user in extra full format:

  ` ps --user $(id -u) -F`

- List all processes of the current user as a tree:

  ` ps --user $(id -u) f`

- Get the parent pid of a process:

  ` ps -o ppid= -p pid`



