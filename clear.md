# Linux clear Command
-------------------
### Command Introduction (命令介绍)
> **clear - clear the terminal screen**
### Command Format and Options (命令格式和选项)
```
#man clear
clear(1)                                                                      General Commands Manual                                                                     clear(1)

NAME
       clear - clear the terminal screen

SYNOPSIS
       clear

DESCRIPTION
       clear  clears  your screen if this is possible.  It looks in the environment for the terminal type and then in the terminfo database to figure out how to clear the screen.
       Some terminals can clear also their scrollback buffer to prevent access to potentially sensitive data.  If the terminfo entry for the terminal type contains extended capa‐
       bility E3, clear will use it to clear the scrollback buffer.

       clear ignores any command-line parameters that may be present.

SEE ALSO
       tput(1), terminfo(5)

       This describes ncurses version 5.9 (patch 20130511).
```
### Command Example (命令范例)
```

  clear

  Clears the screen of the terminal.

  - Clear the screen (equivalent to typing Control-L when using the bash shell):
    clear


```
