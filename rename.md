# Linux rename Command
-------------------
### Command Introduction (命令介绍)
> **rename - rename files**
### Command Format and Options (命令格式和选项)
```
#rename --help

Usage:
 rename [options] expression replacement file...

Options:
 -v, --verbose    explain what is being done
 -s, --symlink    act on symlink target

 -h, --help     display this help and exit
 -V, --version  output version information and exit

For more details see rename(1).
```
### Command Example (命令范例)
```

  rename

  Renames multiple files.

  - Rename files using a Perl Common Regular Expression (substitute 'foo' with 'bar' wherever found):
    rename 's/foo/bar/' *

  - Dry-run - display which renames would occur without performing them:
    rename -n 's/foo/bar/' *

  - Force renaming even if the operation would overwrite existing files:
    rename -f 's/foo/bar/' *

  - Convert filenames to lower case (use -f in case-insensitive filesystems to prevent "already exists" errors):
    rename 'y/A-Z/a-z/' *

  - Replace whitespace with underscores:
    rename 's/\s+/_/g' *


```
