# Linux partprobe Command
-------------------
### Command Introduction (命令介绍)
> **partprobe - inform the OS of partition table changes**
### Command Format and Options (命令格式和选项)
```
#partprobe --help
Usage: partprobe [OPTION] [DEVICE]...
Inform the operating system about partition table changes.

  -d, --dry-run    do not actually inform the operating system
  -s, --summary    print a summary of contents
  -h, --help       display this help and exit
  -v, --version    output version information and exit

When no DEVICE is given, probe all partitions.

Report bugs to <bug-parted@gnu.org>.
```
### Command Example (命令范例)
```
	partprobe
	 - partprobe
	   partprobe
```
