# Linux sed Command
### Command Introduction (命令介绍)
-------------------
> **sed - stream editor for filtering and transforming text**

### Command Format and Options (命令格式和选项)
```
#sed --help
Usage: sed [OPTION]... {script-only-if-no-other-script} [input-file]...

  -n, --quiet, --silent
                 suppress automatic printing of pattern space
  -e script, --expression=script
                 add the script to the commands to be executed
  -f script-file, --file=script-file
                 add the contents of script-file to the commands to be executed
  --follow-symlinks
                 follow symlinks when processing in place
  -i[SUFFIX], --in-place[=SUFFIX]
                 edit files in place (makes backup if SUFFIX supplied)
  -c, --copy
                 use copy instead of rename when shuffling files in -i mode
  -b, --binary
                 does nothing; for compatibility with WIN32/CYGWIN/MSDOS/EMX (
                 open files in binary mode (CR+LFs are not treated specially))
  -l N, --line-length=N
                 specify the desired line-wrap length for the `l' command
  --posix
                 disable all GNU extensions.
  -r, --regexp-extended
                 use extended regular expressions in the script.
  -s, --separate
                 consider files as separate rather than as a single continuous
                 long stream.
  -u, --unbuffered
                 load minimal amounts of data from the input files and flush
                 the output buffers more often
  -z, --null-data
                 separate lines by NUL characters
  --help
                 display this help and exit
  --version
                 output version information and exit

If no -e, --expression, -f, or --file option is given, then the first
non-option argument is taken as the sed script to interpret.  All
remaining arguments are names of input files; if no input files are
specified, then the standard input is read.

GNU sed home page: <http://www.gnu.org/software/sed/>.
General help using GNU software: <http://www.gnu.org/gethelp/>.
E-mail bug reports to: <bug-sed@gnu.org>.
Be sure to include the word ``sed'' somewhere in the ``Subject:'' field.
```
### Command Example (命令范例)
-------------------
**Edit text in a scriptable manner.**

- Replace the first occurrence of a string in a file, and print the result:

  ` sed 's/find/replace/' filename`

- Replace all occurrences of an extended regular expression in a file:

  ` sed -r 's/regex/replace/g' filename`

- Replace all occurrences of a string in a file, overwriting the file (i.e. in-place):

  ` sed -i 's/find/replace/g' filename`

- Replace only on lines matching the line pattern:

  ` sed '/line_pattern/s/find/replace/' filename`

- Delete lines matching the line pattern:

  ` sed '/line_pattern/d' filename`

- Print only text between n-th line till the next empty line:

  ` sed -n 'line_number,/^$/p' filename`

- Apply multiple find-replace expressions to a file:

  ` sed -e 's/find/replace/' -e 's/find/replace/' filename`

- Replace separator / by any other character not used in the find or replace patterns, e.g., #:

  ` sed 's#find#replace#' filename`
