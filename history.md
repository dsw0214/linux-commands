# Linux history Command
-------------------
### Command Introduction (命令介绍)
> **bash, :, ., [, alias, bg, bind, break, builtin, caller, cd, command, compgen, complete, compopt, continue, declare, dirs, disown, echo, enable, eval, exec, exit, export,**
### Command Format and Options (命令格式和选项)
```
history: usage: history [-c] [-d offset] [n] or history -anrw [filename] or history -ps arg [arg...]
```
### Command Example (命令范例)
```

  history

  Command Line history.

  - Display the commands history list with line numbers:
    history

  - Clear the commands history list (only for current bash shell):
    history -c

  - Overwrite history file with history of current bash shell (often combined with history -c to purge history):
    history -w

  - Delete the history entry at the specified offset:
    history -d offset


See also: bash


```
