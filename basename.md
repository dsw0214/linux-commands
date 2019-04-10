# Linux basename Command
-------------------
### Command Introduction (命令介绍)
> **basename - strip directory and suffix from filenames**
### Command Format and Options (命令格式和选项)
```
#basename --help
Usage: basename NAME [SUFFIX]
  or:  basename OPTION... NAME...
Print NAME with any leading directory components removed.
If specified, also remove a trailing SUFFIX.

Mandatory arguments to long options are mandatory for short options too.
  -a, --multiple       support multiple arguments and treat each as a NAME
  -s, --suffix=SUFFIX  remove a trailing SUFFIX
  -z, --zero           separate output with NUL rather than newline
      --help     display this help and exit
      --version  output version information and exit

Examples:
  basename /usr/bin/sort          -> "sort"
  basename include/stdio.h .h     -> "stdio"
  basename -s .h include/stdio.h  -> "stdio"
  basename -a any/str1 any/str2   -> "str1" followed by "str2"

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'basename invocation'
```
### Command Example (命令范例)
```

  basename

  Returns non-directory portion of a pathname.

  - Show only the file name from a path:
    basename path/to/file

  - Show only the file name from a path, with a suffix removed:
    basename path/to/file suffix


```
