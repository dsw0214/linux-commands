# Linux swapon Command
-------------------
### Command Introduction (命令介绍)
> **swapon, swapoff - enable/disable devices and files for paging and swapping**
### Command Format and Options (命令格式和选项)
```
#swapon --help

Usage:
 swapon [options] [<spec>]

Options:
 -a, --all                enable all swaps from /etc/fstab
 -d, --discard[=<policy>] enable swap discards, if supported by device
 -e, --ifexists           silently skip devices that do not exist
 -f, --fixpgsz            reinitialize the swap space if necessary
 -p, --priority <prio>    specify the priority of the swap device
 -s, --summary            display summary about used swap devices
     --show[=<columns>]   display summary in definable table
     --noheadings         don't print headings, use with --show
     --raw                use the raw output format, use with --show
     --bytes              display swap size in bytes in --show output
 -v, --verbose            verbose mode

 -h, --help     display this help and exit
 -V, --version  output version information and exit

The <spec> parameter:
 -L <label>             synonym for LABEL=<label>
 -U <uuid>              synonym for UUID=<uuid>
 LABEL=<label>          specifies device by swap area label
 UUID=<uuid>            specifies device by swap area UUID
 PARTLABEL=<label>      specifies device by partition label
 PARTUUID=<uuid>        specifies device by partition UUID
 <device>               name of device to be used
 <file>                 name of file to be used

Available discard policy types (for --discard):
 once	  : only single-time area discards are issued. (swapon)
 pages	  : discard freed pages before they are reused.
 * if no policy is selected both discard types are enabled. (default)

Available columns (for --show):
 NAME  device file or partition path
 TYPE  type of the device
 SIZE  size of the swap area
 USED  bytes in use
 PRIO  swap priority

For more details see swapon(8).
```
### Command Example (命令范例)
```

  swapon

  Enables device or file for swapping.

  - Get swap information:
    swapon -s

  - Enable a given swap partition:
    swapon /dev/sdb7

  - Enable a given swap file:
    swapon path/to/file

  - Enable all swap areas:
    swapon -a

  - Enable swap by label of a device or file:
    swapon -L swap1


```
