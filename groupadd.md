# Linux groupadd Command
-------------------
### Command Introduction (命令介绍)
> **groupadd - create a new group**
### Command Format and Options (命令格式和选项)
```
#groupadd --help
Usage: groupadd [options] GROUP

Options:
  -f, --force                   exit successfully if the group already exists,
                                and cancel -g if the GID is already used
  -g, --gid GID                 use GID for the new group
  -h, --help                    display this help message and exit
  -K, --key KEY=VALUE           override /etc/login.defs defaults
  -o, --non-unique              allow to create groups with duplicate
                                (non-unique) GID
  -p, --password PASSWORD       use this encrypted password for the new group
  -r, --system                  create a system account
  -R, --root CHROOT_DIR         directory to chroot into

```
### Command Example (命令范例)
```

  groupadd

  Add user groups to the system.

  - Create a new Linux group:
    groupadd group_name

  - Create new group with a specific groupid:
    groupadd group_name -g group_id


```
