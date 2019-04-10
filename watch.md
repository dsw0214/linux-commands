# Linux watch Command
-------------------
### Command Introduction (命令介绍)
> **watch - execute a program periodically, showing output fullscreen**
### Command Format and Options (命令格式和选项)
```
#watch --help

Usage:
 watch [options] command

Options:
  -b, --beep             beep if command has a non-zero exit
  -c, --color            interpret ANSI color and style sequences
  -d, --differences[=<permanent>]
                         highlight changes between updates
  -e, --errexit          exit if command has a non-zero exit
  -g, --chgexit          exit when output from command changes
  -n, --interval <secs>  seconds to wait between updates
  -p, --precise          attempt run command in precise intervals
  -t, --no-title         turn off header
  -x, --exec             pass command to exec instead of "sh -c"

 -h, --help     display this help and exit
 -v, --version  output version information and exit

For more details see watch(1).
```
### Command Example (命令范例)
```

  watch

  Execute a command repeatedly, and monitor the output in full-screen mode.

  - Monitor files in the current directory:
    watch ls

  - Monitor disk space and highlight the changes:
    watch -d df

  - Monitor "node" processes, refreshing every 3 seconds:
    watch -n 3 "ps aux | grep node"


```
