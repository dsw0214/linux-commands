# Linux find Command
### Command Introduction (命令介绍)
-------------------
> ** find - search for files in a directory hierarchy
     information about how unusual characters in filenames are handled.
**
       
### Command Format and Options (命令格式和选项)
```
#find --help
Usage: find [-H] [-L] [-P] [-Olevel] [-D help|tree|search|stat|rates|opt|exec] [path...] [expression]

default path is the current directory; default expression is -print
expression may consist of: operators, options, tests, and actions:

operators (decreasing precedence; -and is implicit where no others are given):
      ( EXPR )   ! EXPR   -not EXPR   EXPR1 -a EXPR2   EXPR1 -and EXPR2
      EXPR1 -o EXPR2   EXPR1 -or EXPR2   EXPR1 , EXPR2

positional options (always true): -daystart -follow -regextype

normal options (always true, specified before other expressions):
      -depth --help -maxdepth LEVELS -mindepth LEVELS -mount -noleaf
      --version -xautofs -xdev -ignore_readdir_race -noignore_readdir_race

tests (N can be +N or -N or N): -amin N -anewer FILE -atime N -cmin N
      -cnewer FILE -ctime N -empty -false -fstype TYPE -gid N -group NAME
      -ilname PATTERN -iname PATTERN -inum N -iwholename PATTERN -iregex PATTERN
      -links N -lname PATTERN -mmin N -mtime N -name PATTERN -newer FILE
      -nouser -nogroup -path PATTERN -perm [-/]MODE -regex PATTERN
      -readable -writable -executable
      -wholename PATTERN -size N[bcwkMG] -true -type [bcdpflsD] -uid N
      -used N -user NAME -xtype [bcdpfls]
      -context CONTEXT


actions: -delete -print0 -printf FORMAT -fprintf FILE FORMAT -print 
      -fprint0 FILE -fprint FILE -ls -fls FILE -prune -quit
      -exec COMMAND ; -exec COMMAND {} + -ok COMMAND ;
      -execdir COMMAND ; -execdir COMMAND {} + -okdir COMMAND ;

Report (and track progress on fixing) bugs via the findutils bug-reporting
page at http://savannah.gnu.org/ or, if you have no web access, by sending
email to <bug-findutils@gnu.org>.
```
### Command Example (命令范例)
-------------------
** Find files or directories under the given directory tree, recursively. **

- Find files by extension:

  ` find root_path -name '*.ext'`

- Find files by matching multiple patterns:

  ` find root_path -name '*pattern_1*' -or -name '*pattern_2*'`

- Find directories matching a given name:

  ` find root_path -type d -name *lib*`

- Find files matching path pattern:

  ` find root_path -path '**/lib/**/*.ext'`

- Run a command for each file, use {} within the command to access the filename:

  ` find root_path -name '*.ext' -exec wc -l {} \;`

- Find files modified in the last 24-hour period:

  ` find root_path -mtime -1`

- Find files using case insensitive name matching, of a certain size:

  ` find root_path -size +500k -size -10M -iname '*.TaR.gZ'`

- Delete files by name, older than 180 days:

  ` find root_path -name '*.ext' -mtime +180 -delete`

- Find files matching a given pattern, while excluding specific paths:

  ` find root_path -name '*.py' -not -path '*/site-packages/*'`

