# Linux touch Command
-------------------
### Command Introduction (命令介绍)
> **touch - change file timestamps**
### Command Format and Options (命令格式和选项)
```
#touch --help
Usage: touch [OPTION]... FILE...
Update the access and modification times of each FILE to the current time.

A FILE argument that does not exist is created empty, unless -c or -h
is supplied.

A FILE argument string of - is handled specially and causes touch to
change the times of the file associated with standard output.

Mandatory arguments to long options are mandatory for short options too.
  -a                     change only the access time
  -c, --no-create        do not create any files
  -d, --date=STRING      parse STRING and use it instead of current time
  -f                     (ignored)
  -h, --no-dereference   affect each symbolic link instead of any referenced
                         file (useful only on systems that can change the
                         timestamps of a symlink)
  -m                     change only the modification time
  -r, --reference=FILE   use this file's times instead of current time
  -t STAMP               use [[CC]YY]MMDDhhmm[.ss] instead of current time
      --time=WORD        change the specified time:
                           WORD is access, atime, or use: equivalent to -a
                           WORD is modify or mtime: equivalent to -m
      --help     display this help and exit
      --version  output version information and exit

Note that the -d and -t options accept different time-date formats.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'touch invocation'
```
### Command Example (命令范例)
```

  touch

  Change a file access and modification times (atime, mtime).

  - Create a new empty file(s) or change the times for existing file(s) to current time:
    touch filename

  - Set the times on a file to a specific date and time:
    touch -t YYYYMMDDHHMM.SS filename

  - Use the times from a file to set the times on a second file:
    touch -r filename filename2


```
