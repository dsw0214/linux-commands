# Linux rm Command
### Command Introduction (命令介绍)
-------------------
> **rm - remove files or directories**

### Command Format and Options (命令格式和选项)
```
#rm --help
Usage: rm [OPTION]... FILE...
Remove (unlink) the FILE(s).

  -f, --force           ignore nonexistent files and arguments, never prompt
  -i                    prompt before every removal
  -I                    prompt once before removing more than three files, or
                          when removing recursively; less intrusive than -i,
                          while still giving protection against most mistakes
      --interactive[=WHEN]  prompt according to WHEN: never, once (-I), or
                          always (-i); without WHEN, prompt always
      --one-file-system  when removing a hierarchy recursively, skip any
                          directory that is on a file system different from
                          that of the corresponding command line argument
      --no-preserve-root  do not treat '/' specially
      --preserve-root   do not remove '/' (default)
  -r, -R, --recursive   remove directories and their contents recursively
  -d, --dir             remove empty directories
  -v, --verbose         explain what is being done
      --help     display this help and exit
      --version  output version information and exit

By default, rm does not remove directories.  Use the --recursive (-r or -R)
option to remove each listed directory, too, along with all of its contents.

To remove a file whose name starts with a '-', for example '-foo',
use one of these commands:
  rm -- -foo

  rm ./-foo

Note that if you use rm to remove a file, it might be possible to recover
some of its contents, given sufficient expertise and/or time.  For greater
assurance that the contents are truly unrecoverable, consider using shred.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'rm invocation'
```
### Command Example (命令范例)
-------------------
**Remove files or directories.**

- Remove files from arbitrary locations:

  ` rm path/to/file path/to/another/file`

- Recursively remove a directory and all its subdirectories:

  ` rm -r path/to/folder`

- Forcibly remove a directory, without prompting for confirmation or showing error messages:

  ` rm -rf path/to/folder`

- Interactively remove multiple files, with a prompt before every removal:

  ` rm -i file(s)`

- Remove files in verbose mode, printing a message for each removed file:

  ` rm -v path/to/folder/*`



