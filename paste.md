# Linux paste Command
-------------------
### Command Introduction (命令介绍)
> **paste - merge lines of files**
### Command Format and Options (命令格式和选项)
```
#paste --help
Usage: paste [OPTION]... [FILE]...
Write lines consisting of the sequentially corresponding lines from
each FILE, separated by TABs, to standard output.
With no FILE, or when FILE is -, read standard input.

Mandatory arguments to long options are mandatory for short options too.
  -d, --delimiters=LIST   reuse characters from LIST instead of TABs
  -s, --serial            paste one file at a time instead of in parallel
      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'paste invocation'
```
### Command Example (命令范例)
```

  paste

  Merge lines of files.

  - Join all the lines into a single line, using TAB as delimiter:
    paste -s file

  - Join all the lines into a single line, using the specified delimiter:
    paste -s -d delimiter file

  - Merge two files side by side, each in its column, using TAB as delimiter:
    paste file1 file2

  - Merge two files side by side, each in its column, using the specified delimiter:
    paste -d delimiter file1 file2

  - Merge two files, with lines added alternatively:
    paste -d '\n' file1 file2


```
