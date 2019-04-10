# Linux sync Command
-------------------
### Command Introduction (命令介绍)
> **sync - flush file system buffers**
### Command Format and Options (命令格式和选项)
```
#sync --help
Usage: sync [OPTION]
Force changed blocks to disk, update the super block.

      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'sync invocation'
```
### Command Example (命令范例)
```

  sync

  Flushes all pending write operations to the appropriate disks.

  - Flush all pending write operations on all disks:
    sync

  - Flush all pending write operations on a single file to disk:
    sync path/to/file


```
