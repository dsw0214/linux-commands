# Linux tree Command
-------------------
### Command Introduction (命令介绍)
> **tree - list contents of directories in a tree-like format.**
### Command Format and Options (命令格式和选项)
```
#tree --help
usage: tree [-acdfghilnpqrstuvxACDFQNSUX] [-H baseHREF] [-T title ] [-L level [-R]]
	[-P pattern] [-I pattern] [-o filename] [--version] [--help] [--inodes]
	[--device] [--noreport] [--nolinks] [--dirsfirst] [--charset charset]
	[--filelimit[=]#] [--si] [--timefmt[=]<f>] [<directory list>]
  ------- Listing options -------
  -a            All files are listed.
  -d            List directories only.
  -l            Follow symbolic links like directories.
  -f            Print the full path prefix for each file.
  -x            Stay on current filesystem only.
  -L level      Descend only level directories deep.
  -R            Rerun tree when max dir level reached.
  -P pattern    List only those files that match the pattern given.
  -I pattern    Do not list files that match the given pattern.
  --noreport    Turn off file/directory count at end of tree listing.
  --charset X   Use charset X for terminal/HTML and indentation line output.
  --filelimit # Do not descend dirs with more than # files in them.
  --timefmt <f> Print and format time according to the format <f>.
  -o filename   Output to file instead of stdout.
  --du          Print directory sizes.
  --prune       Prune empty directories from the output.
  -------- File options ---------
  -q            Print non-printable characters as '?'.
  -N            Print non-printable characters as is.
  -Q            Quote filenames with double quotes.
  -p            Print the protections for each file.
  -u            Displays file owner or UID number.
  -g            Displays file group owner or GID number.
  -s            Print the size in bytes of each file.
  -h            Print the size in a more human readable way.
  --si          Like -h, but use in SI units (powers of 1000).
  -D            Print the date of last modification or (-c) status change.
  -F            Appends '/', '=', '*', '@', '|' or '>' as per ls -F.
  --inodes      Print inode number of each file.
  --device      Print device ID number to which each file belongs.
  ------- Sorting options -------
  -v            Sort files alphanumerically by version.
  -r            Sort files in reverse alphanumeric order.
  -t            Sort files by last modification time.
  -c            Sort files by last status change time.
  -U            Leave files unsorted.
  --dirsfirst   List directories before files (-U disables).
  ------- Graphics options ------
  -i            Don't print indentation lines.
  -A            Print ANSI lines graphic indentation lines.
  -S            Print with ASCII graphics indentation lines.
  -n            Turn colorization off always (-C overrides).
  -C            Turn colorization on always.
  ------- XML/HTML options -------
  -X            Prints out an XML representation of the tree.
  -H baseHREF   Prints out HTML format with baseHREF as top directory.
  -T string     Replace the default HTML title and H1 header with string.
  --nolinks     Turn off hyperlinks in HTML output.
  ---- Miscellaneous options ----
  --version     Print version and exit.
  --help        Print usage and this help message and exit.
```
### Command Example (命令范例)
```

  tree

  Show the contents of the current directory as a tree.

  - Show files and directories up to 'num' levels of depth (where 1 means the current directory):
    tree -L num

  - Show directories only:
    tree -d

  - Show hidden files too:
    tree -a

  - Print the tree without indentation lines, showing the full path instead (use -N to not escape whitespace and special characters):
    tree -i -f

  - Print the size of each node next to it, in human-readable format:
    tree -s -h

  - Filter the tree using a wildcard (glob) pattern:
    tree -P *.txt

  - Ignore entries that match a wildcard (glob) pattern:
    tree -I *.txt


```
