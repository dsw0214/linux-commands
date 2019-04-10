# Linux vimdiff Command
-------------------
### Command Introduction (命令介绍)
> **vimdiff - edit two, three or four versions of a file with Vim and show differences**
### Command Format and Options (命令格式和选项)
```
#vimdiff --help
VIM - Vi IMproved 7.4 (2013 Aug 10, compiled Aug  2 2017 00:45:39)

usage: vim [arguments] [file ..]       edit specified file(s)
   or: vim [arguments] -               read text from stdin
   or: vim [arguments] -t tag          edit file where tag is defined
   or: vim [arguments] -q [errorfile]  edit file with first error

Arguments:
   --			Only file names after this
   -v			Vi mode (like "vi")
   -e			Ex mode (like "ex")
   -E			Improved Ex mode
   -s			Silent (batch) mode (only for "ex")
   -d			Diff mode (like "vimdiff")
   -y			Easy mode (like "evim", modeless)
   -R			Readonly mode (like "view")
   -Z			Restricted mode (like "rvim")
   -m			Modifications (writing files) not allowed
   -M			Modifications in text not allowed
   -b			Binary mode
   -l			Lisp mode
   -C			Compatible with Vi: 'compatible'
   -N			Not fully Vi compatible: 'nocompatible'
   -V[N][fname]		Be verbose [level N] [log messages to fname]
   -D			Debugging mode
   -n			No swap file, use memory only
   -r			List swap files and exit
   -r (with file name)	Recover crashed session
   -L			Same as -r
   -A			start in Arabic mode
   -H			Start in Hebrew mode
   -F			Start in Farsi mode
   -T <terminal>	Set terminal type to <terminal>
   -u <vimrc>		Use <vimrc> instead of any .vimrc
   --noplugin		Don't load plugin scripts
   -p[N]		Open N tab pages (default: one for each file)
   -o[N]		Open N windows (default: one for each file)
   -O[N]		Like -o but split vertically
   +			Start at end of file
   +<lnum>		Start at line <lnum>
   --cmd <command>	Execute <command> before loading any vimrc file
   -c <command>		Execute <command> after loading the first file
   -S <session>		Source file <session> after loading the first file
   -s <scriptin>	Read Normal mode commands from file <scriptin>
   -w <scriptout>	Append all typed commands to file <scriptout>
   -W <scriptout>	Write all typed commands to file <scriptout>
   -x			Edit encrypted files
   --startuptime <file>	Write startup timing messages to <file>
   -i <viminfo>		Use <viminfo> instead of .viminfo
   -h  or  --help	Print Help (this message) and exit
   --version		Print version information and exit
```
### Command Example (命令范例)
```

  vimdiff

  Open up to four files in vim and show the differences between them.
  See vim documentation for working with files and navigating within a window.

  - Open two files and show the differences (up to four files can be compared):
    vimdiff file1 file2

  - Open two files using a horizontal window split instead of the default vertical split:
    vimdiff -o file1 file2

  - Move the cursor to the window on the left|right|up|down:
    Ctrl + w h|l|k|j


See also: vim


```
