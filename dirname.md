# Linux dirname Command
-------------------
### Command Introduction (命令介绍)
> **dirname - strip last component from file name**
### Command Format and Options (命令格式和选项)
```
#dirname --help
Usage: dirname [OPTION] NAME...
Output each NAME with its last non-slash component and trailing slashes
removed; if NAME contains no /'s, output '.' (meaning the current directory).

  -z, --zero     separate output with NUL rather than newline
      --help     display this help and exit
      --version  output version information and exit

Examples:
  dirname /usr/bin/          -> "/usr"
  dirname dir1/str dir2/str  -> "dir1" followed by "dir2"
  dirname stdio.h            -> "."

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'dirname invocation'
```
### Command Example (命令范例)
```

  dirname

  Calculates the parent directory of a given file or directory path.

  - Calculate the parent directory of a given path:
    dirname path/to/file_or_directory

  - Calculate the parent directory of multiple paths:
    dirname path/to/file_a path/to/directory_b

  - Delimit output with a NUL character instead of a newline (useful when combining with xargs):
    dirname --zero path/to/directory_a path/to/file_b


See also: xargs


```
