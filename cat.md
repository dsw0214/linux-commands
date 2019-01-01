# Linux cat Command
### Command Introduction (命令介绍)
-------------------
> **cat - concatenate files and print on the standard output**

### Command Format and Options (命令格式和选项)
```
#cat --help
Usage: cat [OPTION]... [FILE]...
Concatenate FILE(s), or standard input, to standard output.

  -A, --show-all           equivalent to -vET
  -b, --number-nonblank    number nonempty output lines, overrides -n
  -e                       equivalent to -vE
  -E, --show-ends          display $ at end of each line
  -n, --number             number all output lines
  -s, --squeeze-blank      suppress repeated empty output lines
  -t                       equivalent to -vT
  -T, --show-tabs          display TAB characters as ^I
  -u                       (ignored)
  -v, --show-nonprinting   use ^ and M- notation, except for LFD and TAB
      --help     display this help and exit
      --version  output version information and exit

With no FILE, or when FILE is -, read standard input.

Examples:
  cat f - g  Output f's contents, then standard input, then g's contents.
  cat        Copy standard input to standard output.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'cat invocation'
```
### Command Example (命令范例)
-------------------
**Print and concatenate files.**

- Print the contents of a file to the standard output:

  ` cat file`

- Concatenate several files into the target file:

  ` cat file1 file2 > target_file`

- Append several files into the target file:

  ` cat file1 file2 >> target_file`

- Number all output lines:

  ` cat -n file`
