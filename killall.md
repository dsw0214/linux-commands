# Linux killall Command
-------------------
### Command Introduction (命令介绍)
> **killall - kill processes by name**
### Command Format and Options (命令格式和选项)
```
# killall --help
Usage: killall [-Z CONTEXT] [-u USER] [ -eIgiqrvw ] [ -SIGNAL ] NAME...
       killall -l, --list
       killall -V, --version

  -e,--exact          require exact match for very long names
  -I,--ignore-case    case insensitive process name match
  -g,--process-group  kill process group instead of process
  -y,--younger-than   kill processes younger than TIME
  -o,--older-than     kill processes older than TIME
  -i,--interactive    ask for confirmation before killing
  -l,--list           list all known signal names
  -q,--quiet          don't print complaints
  -r,--regexp         interpret NAME as an extended regular expression
  -s,--signal SIGNAL  send this signal instead of SIGTERM
  -u,--user USER      kill only process(es) running as USER
  -v,--verbose        report if the signal was successfully sent
  -V,--version        display version information
  -w,--wait           wait for processes to die
  -Z,--context REGEXP kill only process(es) having context
                      (must precede other arguments)
```
### Command Example (命令范例)
```
killall

  Send kill signal to all instances of a process by name (must be exact name).
  All signals except SIGKILL and SIGSTOP can be intercepted by the process, allowing a clean exit.

  - Terminate a process using the default SIGTERM (terminate) signal:
    killall process_name

  - List available signal names (to be used without the 'SIG' prefix):
    killall --list

  - Interactively ask for confirmation before termination:
    killall -i process_name

  - Terminate a process using the SIGINT (interrupt) signal, which is the same signal sent by pressing Ctrl + C:
    killall -INT process_name

  - Force kill a process:
    killall -KILL process_name

```
