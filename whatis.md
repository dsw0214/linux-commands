# Linux whatis Command
### Command Introduction (命令介绍)
-------------------
> ** whatis - display manual page descriptions **

### Command Format and Options (命令格式和选项)
```
#whatis --help
Usage: whatis [OPTION...] KEYWORD...

  -d, --debug                emit debugging messages
  -v, --verbose              print verbose warning messages
  -r, --regex                interpret each keyword as a regex
  -w, --wildcard             the keyword(s) contain wildcards
  -l, --long                 do not trim output to terminal width
  -C, --config-file=FILE     use this user configuration file
  -L, --locale=LOCALE        define the locale for this search
  -m, --systems=SYSTEM       use manual pages from other systems
  -M, --manpath=PATH         set search path for manual pages to PATH
  -s, --sections=LIST, --section=LIST
                             search only these sections (colon-separated)
  -?, --help                 give this help list
      --usage                give a short usage message
  -V, --version              print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Report bugs to cjwatson@debian.org.
```

### Command Example (命令范例)
-------------------
** Display one-line descriptions from manual pages. **

- Display a description from a man page:

  ` whatis command`

- Don't cut the description off at the end of the line:

  ` whatis --long command`

- Display descriptions for all commands matching a glob:

  ` whatis --wildcard net*`

- Search man page descriptions with a regular expression:

  ` whatis --regex 'wish[0-9]\.[0-9]'`
