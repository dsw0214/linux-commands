# Linux userdel Command
-------------------
### Command Introduction (命令介绍)
> **userdel - delete a user account and related files**
### Command Format and Options (命令格式和选项)
```
#userdel --help
Usage: userdel [options] LOGIN

Options:
  -f, --force                   force some actions that would fail otherwise
                                e.g. removal of user still logged in
                                or files, even if not owned by the user
  -h, --help                    display this help message and exit
  -r, --remove                  remove home directory and mail spool
  -R, --root CHROOT_DIR         directory to chroot into
  -Z, --selinux-user            remove any SELinux user mapping for the user

```
### Command Example (命令范例)
```

  userdel

  Remove a user.

  - Remove a user and their home directory:
    userdel -r name


```
