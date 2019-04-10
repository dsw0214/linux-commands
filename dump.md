# Linux dump Command
-------------------
### Command Introduction (命令介绍)
> **dig - DNS lookup utility**
### Command Format and Options (命令格式和选项)
```
#dump --help
dump [-level#] [-acmMnqSuv] [-A file] [-B records] [-b blocksize]

[-d density] [-D file] [-e inode#,inode#,...] [-E file]

[-f file] [-h level] [-I nr errors] [-j zlevel] [-Q file]

[-s feet] [-T date] [-y] [-z zlevel] filesystem
```
### Command Example (命令范例)
```

  #dump

  - Before full backup /dev/sda1, count the capacity required
  dump –0s /dev/sda1

```
