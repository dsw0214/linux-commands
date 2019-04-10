# Linux tac Command
-------------------
### Command Introduction (命令介绍)
> **tac - concatenate and print files in reverse**
### Command Format and Options (命令格式和选项)
```
#tac --help
Usage: tac [OPTION]... [FILE]...
Write each FILE to standard output, last line first.
With no FILE, or when FILE is -, read standard input.

Mandatory arguments to long options are mandatory for short options too.
  -b, --before             attach the separator before instead of after
  -r, --regex              interpret the separator as a regular expression
  -s, --separator=STRING   use STRING as the separator instead of newline
      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'tac invocation'
```
### Command Example (命令范例)
```

  tac

  Print and concatenate files in reverse.

  - Print the contents of file1 reversed to the standard output:
    tac file1

  - Concatenate several files reversed into the target file:
    tac file1 file2 > target_file


```
