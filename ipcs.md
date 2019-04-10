# Linux ipcs Command
-------------------
### Command Introduction (命令介绍)
> **ipcs - provide information on IPC facilities**
### Command Format and Options (命令格式和选项)
```
#ipcs --help

Usage:
 ipcs [resource ...] [output-format]
 ipcs [resource] -i <id>

Options:
 -i, --id <id>  print details on resource identified by id
 -h, --help     display this help and exit
 -V, --version  output version information and exit

Resource options:
 -m, --shmems      shared memory segments
 -q, --queues      message queues
 -s, --semaphores  semaphores
 -a, --all         all (default)

Output format:
 -t, --time        show attach, detach and change times
 -p, --pid         show creator and last operations PIDs
 -c, --creator     show creator and owner
 -l, --limits      show resource limits
 -u, --summary     show status summary
     --human       show sizes in human readable format
 -b, --bytes       show sizes in bytes

For more details see ipcs(1).
```
### Command Example (命令范例)
```

  ipcs

  Display information about resources used in IPC (Inter-process Communication).

  - Specific information about the Message Queue which has the id 32768:
    ipcs -qi 32768

  - General information about all the IPC:
    ipcs -a


```
