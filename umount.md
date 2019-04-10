# Linux umount Command
-------------------
### Command Introduction (命令介绍)
> **umount - unmount file systems**
### Command Format and Options (命令格式和选项)
```
#umount --help

Usage:
 umount [-hV]
 umount -a [options]
 umount [options] <source> | <directory>

Options:
 -a, --all               unmount all filesystems
 -A, --all-targets       unmount all mountpoins for the given device
                         in the current namespace
 -c, --no-canonicalize   don't canonicalize paths
 -d, --detach-loop       if mounted loop device, also free this loop device
     --fake              dry run; skip the umount(2) syscall
 -f, --force             force unmount (in case of an unreachable NFS system)
 -i, --internal-only     don't call the umount.<type> helpers
 -n, --no-mtab           don't write to /etc/mtab
 -l, --lazy              detach the filesystem now, and cleanup all later
 -O, --test-opts <list>  limit the set of filesystems (use with -a)
 -R, --recursive         recursively unmount a target with all its children
 -r, --read-only         In case unmounting fails, try to remount read-only
 -t, --types <list>      limit the set of filesystem types
 -v, --verbose           say what is being done

 -h, --help     display this help and exit
 -V, --version  output version information and exit

For more details see umount(8).
```
### Command Example (命令范例)
```

  umount

  Unlink a filesystem from its mount point, making it no longer accessible.
  A filesystem cannot be unmounted when it is busy.

  - Unmount a filesystem, by passing the path to the source it is mounted from:
    umount path/to/device_file

  - Unmount a filesystem, by passing the path to the target where it is mounted:
    umount path/to/mounted_directory

  - Unmount all mounted filesystems (except the proc filesystem):
    umount -a


```
