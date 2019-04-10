# Linux e2fsck Command
-------------------
### Command Introduction (命令介绍)
> **e2fsck - check a Linux ext2/ext3/ext4 file system**
### Command Format and Options (命令格式和选项)
```
Usage: e2fsck [-panyrcdfvtDFV] [-b superblock] [-B blocksize]
```
### Command Example (命令范例)
```
	- Check whether / dev / hda5 is normal, if there is an exception, 
	- it will be automatically repaired, and set if there is a question and answer, all answer [yes]:
	e2fsck -a -y /dev/hda5

```
