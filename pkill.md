# Linux pkill Command
-------------------
### Command Introduction (命令介绍)
> **pgrep, pkill - look up or signal processes based on name and other attributes**
### Command Format and Options (命令格式和选项)
```
#pkill --help

Usage:
 pkill [options] <pattern>

Options:
 -<sig>, --signal <sig>    signal to send (either number or name)
 -e, --echo                display what is killed
 -c, --count               count of matching processes
 -f, --full                use full process name to match
 -g, --pgroup <PGID,...>   match listed process group IDs
 -G, --group <GID,...>     match real group IDs
 -n, --newest              select most recently started
 -o, --oldest              select least recently started
 -P, --parent <PPID,...>   match only child processes of the given parent
 -s, --session <SID,...>   match session IDs
 -t, --terminal <tty,...>  match by controlling terminal
 -u, --euid <ID,...>       match by effective IDs
 -U, --uid <ID,...>        match by real IDs
 -x, --exact               match exactly with the command name
 -F, --pidfile <file>      read PIDs from file
 -L, --logpidfile          fail if PID file is not locked
 --ns <PID>                match the processes that belong to the same
                           namespace as <pid>
 --nslist <ns,...>         list which namespaces will be considered for
                           the --ns option.
                           Available namespaces: ipc, mnt, net, pid, user, uts

 -h, --help     display this help and exit
 -V, --version  output version information and exit

For more details see pgrep(1).
```
### Command Example (命令范例)
```

  pkill

  Signal process by name.
  Mostly used for stopping processes.

  - Kill all processes which match:
    pkill -9 process_name

  - Kill all processes which match their full command instead of just the process name:
    pkill -9 -f "command_name"

  - Send SIGUSR1 signal to processes which match:
    pkill -USR1 process_name


```
