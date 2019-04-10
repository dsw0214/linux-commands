# Linux nohup Command
-------------------
### Command Introduction (命令介绍)
> **nohup - run a command immune to hangups, with output to a non-tty**
### Command Format and Options (命令格式和选项)
```
#nohup --help
Usage: nohup COMMAND [ARG]...
  or:  nohup OPTION
Run COMMAND, ignoring hangup signals.

      --help     display this help and exit
      --version  output version information and exit

If standard input is a terminal, redirect it from /dev/null.
If standard output is a terminal, append output to 'nohup.out' if possible,
'$HOME/nohup.out' otherwise.
If standard error is a terminal, redirect it to standard output.
To save output to FILE, use 'nohup COMMAND > FILE'.

NOTE: your shell may have its own version of nohup, which usually supersedes
the version described here.  Please refer to your shell's documentation
for details about the options it supports.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'nohup invocation'
```
### Command Example (命令范例)
```
   nohup

  Allows for a process to live when the terminal gets killed.

  - Run process that can live beyond the terminal:
    nohup command options

```
