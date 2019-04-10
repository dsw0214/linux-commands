# Linux alias Command
-------------------
### Command Introduction (命令介绍)
> **bash, :, ., [, alias, bg, bind, break, builtin, caller, cd, command, compgen, complete, compopt, continue, declare, dirs, disown, echo, enable, eval, exec, exit, export,**
### Command Format and Options (命令格式和选项)
```
alias: usage: alias [-p] [name[=value] ... ]
```
### Command Example (命令范例)
```

  alias

  Creates aliases -- words that are replaced by a command string.
  Aliases expire with the current shell session, unless they're defined in the shell's configuration file, e.g. ~/.bashrc.

  - Create a generic alias:
    alias word="command"

  - View the command associated to a given alias:
    alias word

  - Remove an aliased command:
    unalias word

  - List all aliased words:
    alias -p

  - Turn rm into an interactive command:
    alias rm="rm -i"

  - Create la as a shortcut for ls -a:
    alias la="ls -a"


```
