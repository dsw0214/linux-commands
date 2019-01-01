# Linux whereis Command
### Command Introduction (命令介绍)
-------------------
> **whereis - locate the binary, source, and manual page files for a command**

### Command Format and Options (命令格式和选项)
```
#whereis --help
Usage:
 whereis [options] file

Options:
 -b         search only for binaries
 -B <dirs>  define binaries lookup path
 -m         search only for manuals
 -M <dirs>  define man lookup path
 -s         search only for sources
 -S <dirs>  define sources lookup path
 -f         terminate <dirs> argument list
 -u         search for unusual entries
 -l         output effective lookup paths

For more details see whereis(1).
```
### Command Example (命令范例)
-------------------
**Locate the binary, source, and manual page files for a command.**

- Locate binary, source and man pages for ssh:

  ` whereis ssh`

- Locate binary and man pages for ls:

  ` whereis -bm ls`

- Locate source of gcc and man pages for git:

  ` whereis -s gcc -m git`

- Locate binaries for gcc in /usr/bin/ only:

  ` whereis -b -B /usr/bin/ -f gcc`
