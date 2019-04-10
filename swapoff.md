# Linux swapoff Command
-------------------
### Command Introduction (命令介绍)
> **swapon, swapoff - enable/disable devices and files for paging and swapping**
### Command Format and Options (命令格式和选项)
```
#swapoff --help

Usage:
 swapoff [options] [<spec>]

Options:
 -a, --all              disable all swaps from /proc/swaps
 -v, --verbose          verbose mode

 -h, --help     display this help and exit
 -V, --version  output version information and exit

The <spec> parameter:
 -L <label>             LABEL of device to be used
 -U <uuid>              UUID of device to be used
 LABEL=<label>          LABEL of device to be used
 UUID=<uuid>            UUID of device to be used
 <device>               name of device to be used
 <file>                 name of file to be used

For more details see swapoff(8).
```
### Command Example (命令范例)
```

  swapoff

  Disables device or file for swapping.

  - Disable a given swap partition:
    swapoff /dev/sdb7

  - Disable a given swap file:
    swapoff path/to/file

  - Disable all swap areas:
    swapoff -a

  - Disable swap by label of a device or file:
    swapoff -L swap1


```
