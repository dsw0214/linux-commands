# Linux chmod Command
### Command Introduction (命令介绍)
-------------------
> ** chmod - change file mode bits **

### Command Format and Options (命令格式和选项)
```
#chmod --help
Usage: chmod [OPTION]... MODE[,MODE]... FILE...
  or:  chmod [OPTION]... OCTAL-MODE FILE...
  or:  chmod [OPTION]... --reference=RFILE FILE...
Change the mode of each FILE to MODE.
With --reference, change the mode of each FILE to that of RFILE.

  -c, --changes          like verbose but report only when a change is made
  -f, --silent, --quiet  suppress most error messages
  -v, --verbose          output a diagnostic for every file processed
      --no-preserve-root  do not treat '/' specially (the default)
      --preserve-root    fail to operate recursively on '/'
      --reference=RFILE  use RFILE's mode instead of MODE values
  -R, --recursive        change files and directories recursively
      --help     display this help and exit
      --version  output version information and exit

Each MODE is of the form '[ugoa]*([-+=]([rwxXst]*|[ugo]))+|[-+=][0-7]+'.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'chmod invocation'
```
### Command Example (命令范例)
-------------------
** Change the access permissions of a file or directory. **

- Give the [u]ser who owns a file the right to e[x]ecute it:

  ` chmod u+x file`

- Give the user rights to [r]ead and [w]rite to a file/directory:

  ` chmod u+rw file`

- Remove executable rights from the [g]roup:

  ` chmod g-x file`

- Give [a]ll users rights to read and execute:

  ` chmod a+rx file`

- Give [o]thers (not in the file owner's group) the same rights as the group:

  ` chmod o=g file`

- Change permissions recursively giving [g]roup and [o]thers the abililty to [w]rite:

  ` chmod -R g+w,o+w directory`
