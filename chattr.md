# Linux chattr Command
-------------------
### Command Introduction (命令介绍)
> **chattr - change file attributes on a Linux file system**
### Command Format and Options (命令格式和选项)
```
#chattr --help
Usage: chattr [-RVf] [-+=aAcCdDeijsStTu] [-v version] files...
```
### Command Example (命令范例)
```

  chattr

  Change attributes of files or directories.

  - Make a file or directory immutable to changes and deletion, even by superuser:
    chattr +i path/to/file_or_directory

  - Make a file or directory mutable:
    chattr -i path/to/file_or_directory

  - Recursively make an entire directory and contents immutable:
    chattr -R +i path/to/directory


```
