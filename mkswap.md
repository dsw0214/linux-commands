# Linux mkswap Command
-------------------
### Command Introduction (命令介绍)
> **mkswap - set up a Linux swap area**
### Command Format and Options (命令格式和选项)
```
#mkswap --help

Usage:
 mkswap [options] device [size]

Options:
 -c, --check               check bad blocks before creating the swap area
 -f, --force               allow swap size area be larger than device
 -p, --pagesize SIZE       specify page size in bytes
 -L, --label LABEL         specify label
 -v, --swapversion NUM     specify swap-space version number
 -U, --uuid UUID           specify the uuid to use
 -V, --version             output version information and exit
 -h, --help                display this help and exit

```
### Command Example (命令范例)
```

  mkswap

  Sets up a Linux swap area on a device or in a file.

  - Setup a given partition as swap area:
    sudo mkswap /dev/sdb7

  - Use a given file as swap area:
    sudo mkswap path/to/file

  - Check a partition for bad blocks before creating the swap area:
    sudo mkswap -c /dev/sdb7

  - Specify a label for the file (to allow swapon to use the label):
    sudo mkswap -L swap1 path/to/file


See also: swapon


```
