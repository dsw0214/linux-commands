# Linux eject Command
-------------------
### Command Introduction (命令介绍)
> **eject - eject removable media**
### Command Format and Options (命令格式和选项)
```
#eject --help

Usage:
 eject [options] [<device>|<mountpoint>]

Options:
 -a, --auto <on|off>         turn auto-eject feature on or off
 -c, --changerslot <slot>    switch discs on a CD-ROM changer
 -d, --default               display default device
 -f, --floppy                eject floppy
 -F, --force                 don't care about device type
 -i, --manualeject <on|off>  toggle manual eject protection on/off
 -m, --no-unmount            do not unmount device even if it is mounted
 -M, --no-partitions-unmount do not unmount another partitions
 -n, --noop                  don't eject, just show device found
 -p, --proc                  use /proc/mounts instead of /etc/mtab
 -q, --tape                  eject tape
 -r, --cdrom                 eject CD-ROM
 -s, --scsi                  eject SCSI device
 -t, --trayclose             close tray
 -T, --traytoggle            toggle tray
 -v, --verbose               enable verbose output
 -x, --cdspeed <speed>       set CD-ROM max speed
 -X, --listspeed             list CD-ROM available speeds

 -h, --help     display this help and exit
 -V, --version  output version information and exit

By default tries -r, -s, -f, and -q in order until success.

For more details see eject(1).
```
### Command Example (命令范例)
```

  eject

  Eject cds, floppy disks and tape drives.

  - Display the default device:
    eject -d

  - Eject the default device:
    eject

  - Eject a specific device (the default order is cd-rom, scsi, floppy and tape):
    eject /dev/cdrom

  - Toggle whether a device's tray is open or closed:
    eject -T /dev/cdrom

  - Eject a cd drive:
    eject -r /dev/cdrom

  - Eject a floppy drive:
    eject -f /mnt/floppy

  - Eject a tape drive:
    eject -q /mnt/tape


```
