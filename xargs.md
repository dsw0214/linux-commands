# Linux xargs Command
-------------------
### Command Introduction (命令介绍)
> **xargs - build and execute command lines from standard input**
### Command Format and Options (命令格式和选项)
```
#xargs --help
Usage: xargs [OPTION]... COMMAND INITIAL-ARGS...
Run COMMAND with arguments INITIAL-ARGS and more arguments read from input.

Mandatory arguments to long options are mandatory for short options too.
Non-mandatory arguments are indicated by [square brackets]
  -0, --null                   Items are separated by a null, not whitespace.
                               Disables quote and backslash processing
  -a, --arg-file=FILE          Read arguments from FILE, not standard input
  -d, --delimiter=CHARACTER    Input items are separated by CHARACTER, not by
                               blank space. Disables quote and backslash
                               processing
  -E END                       If END occurs as a line of input, the rest of
                               the input is ignored.
  -e [END], --eof[=END]        Equivalent to -E END if END is specified.
                               Otherwise, there is no end-of-file string
  --help                       Print a summary of the options to xargs.
  -I R                         same as --replace=R (R must be specified)
  -i,--replace=[R]             Replace R in initial arguments with names
                               read from standard input. If R is
                               unspecified, assume {}
  -L,-l, --max-lines=MAX-LINES Use at most MAX-LINES nonblank input lines per
                               command line
  -l                           Use at most one nonblank input line per
                               command line
  -n, --max-args=MAX-ARGS      Use at most MAX-ARGS arguments per command
                               line
  -P, --max-procs=MAX-PROCS    Run up to max-procs processes at a time
  -p, --interactive            Prompt before running commands
  --process-slot-var=VAR       Set environment variable VAR in child
                               processes
  -r, --no-run-if-empty        If there are no arguments, run no command.
                               If this option is not given, COMMAND will be
                               run at least once.
  -s, --max-chars=MAX-CHARS    Limit commands to MAX-CHARS at most
  --show-limits                Show limits on command-line length.
  -t, --verbose                Print commands before executing them
  --version                    Print the version number
  -x, --exit                   Exit if the size (see -s) is exceeded

Report bugs to <bug-findutils@gnu.org>.
```
### Command Example (命令范例)
```

  xargs

  Execute a command with piped arguments coming from another command, a file, etc.
  The input is treated as a single block of text and split into separate arguments on spaces, tabs, newlines and end-of-file.

  - Main usage pattern:
    arguments_source | xargs command

  - Delete all files with a .backup extension. -print0 on find uses a null character to split the files, and -0 changes the delimiter to the null character (useful if there's whitespace in filenames):
    find . -name '*.backup' -print0 | xargs -0 rm -v

  - Execute the command once for each input line, replacing any occurrences of the placeholder (here marked as _) with the input line:
    arguments_source | xargs -I _ command _ optional_extra_arguments

  - Parallel runs of up to max-procs processes at a time; the default is 1. If max-procs is 0, xargs will run as many processes as possible at a time:
    arguments_source | xargs -P max-procs command


```
