# Linux rev Command
-------------------
### Command Introduction (命令介绍)
> **rev - reverse lines of a file or files**
### Command Format and Options (命令格式和选项)
```
#rev --help
Usage: rev [options] [file ...]

Options:
 -V, --version   output version information and exit
 -h, --help      display this help and exit

For more information see rev(1).
```
### Command Example (命令范例)
```

  rev

  Reverse a line of text.

  - Reverse the text string "hello":
    echo "hello" | rev

  - Reverse an entire file and print to stdout:
    rev file


```
