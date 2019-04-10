# Linux visudo Command
-------------------
### Command Introduction (命令介绍)
> **SYNOPSIS**
### Command Format and Options (命令格式和选项)
```
#visudo --help
visudo - safely edit the sudoers file

usage: visudo [-chqsV] [-f sudoers] [-x output_file]

Options:
  -c, --check              check-only mode
  -f, --file=sudoers       specify sudoers file location
  -h, --help               display help message and exit
  -q, --quiet              less verbose (quiet) syntax error messages
  -s, --strict             strict syntax checking
  -V, --version            display version information and exit
  -x, --export=output_file write sudoers in JSON format to output_file
```
### Command Example (命令范例)
```

  visudo

  Safely edit the sudoers file.

  - Edit sudoers file:
    sudo visudo

  - Check sudoers file for errors:
    sudo visudo -c


```
