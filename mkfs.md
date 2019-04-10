# Linux mkfs Command
-------------------
### Command Introduction (命令介绍)
> **mkfs - build a Linux filesystem**
### Command Format and Options (命令格式和选项)
```
#mkfs --help
Usage:
 mkfs [options] [-t <type>] [fs-options] <device> [<size>]

Options:
 -t, --type=<type>  filesystem type; when unspecified, ext2 is used
     fs-options     parameters for the real filesystem builder
     <device>       path to the device to be used
     <size>         number of blocks to be used on the device
 -V, --verbose      explain what is being done;
                      specifying -V more than once will cause a dry-run
 -V, --version      display version information and exit;
                      -V as --version must be the only option
 -h, --help         display this help text and exit

For more information see mkfs(8).
```
### Command Example (命令范例)
```
	mfks 
	- Format sda6 partitions into ext3 format
		mfks -t ext3 /dev/sda6  
	   
	- Format sda7 partitions into ext2 format
	    mkfs -t ext2 /dev/sda7   
    
```
