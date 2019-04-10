# Linux fsck Command
-------------------
### Command Introduction (命令介绍)
> **fsck - check and repair a Linux filesystem**
### Command Format and Options (命令格式和选项)
```
#fsck --help
fsck from util-linux 2.23.2
```
### Command Example (命令范例)
```

  fsck

  Check the integrity of a filesystem or repair it. The filesystem should be unmounted at the time the command is run.

  - Check filesystem /dev/sda, reporting any damaged blocks:
    fsck /dev/sda

  - Check filesystem /dev/sda, reporting any damaged blocks and interactively letting the user choose to repair each one:
    fsck -r /dev/sda

  - Check filesystem /dev/sda, reporting any damaged blocks and automatically repairing them:
    fsck -a /dev/sda


```
