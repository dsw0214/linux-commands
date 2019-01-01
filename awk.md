# Linux awk Command
### Command Introduction (命令介绍)
-------------------
> **  gawk - pattern scanning and processing language **

### Command Format and Options (命令格式和选项)
```
#awk --help
Usage: awk [POSIX or GNU style options] -f progfile [--] file ...
Usage: awk [POSIX or GNU style options] [--] 'program' file ...
POSIX options:		GNU long options: (standard)
	-f progfile		--file=progfile
	-F fs			--field-separator=fs
	-v var=val		--assign=var=val
Short options:		GNU long options: (extensions)
	-b			--characters-as-bytes
	-c			--traditional
	-C			--copyright
	-d[file]		--dump-variables[=file]
	-e 'program-text'	--source='program-text'
	-E file			--exec=file
	-g			--gen-pot
	-h			--help
	-L [fatal]		--lint[=fatal]
	-n			--non-decimal-data
	-N			--use-lc-numeric
	-O			--optimize
	-p[file]		--profile[=file]
	-P			--posix
	-r			--re-interval
	-S			--sandbox
	-t			--lint-old
	-V			--version

To report bugs, see node `Bugs' in `gawk.info', which is
section `Reporting Problems and Bugs' in the printed version.

gawk is a pattern scanning and processing language.
By default it reads standard input and writes standard output.

Examples:
	gawk '{ sum += $1 }; END { print sum }' file
	gawk -F: '{ print $1 }' /etc/passwd
```
### Command Example (命令范例)
-------------------
** A versatile programming language for working on files. **

- Print the fifth column (a.k.a. field) in a space-separated file:

  ` awk '{print $5}' filename`

- Print the second column of the lines containing "something" in a space-separated file:

  ` awk '/something/ {print $2}' filename`

- Print the last column of each line in a file, using a comma (instead of space) as a field separator:

  ` awk -F ',' '{print $NF}' filename`

- Sum the values in the first column of a file and print the total:

  ` awk '{s+=$1} END {print s}' filename`

- Sum the values in the first column and pretty-print the values and then the total:

  ` awk '{s+=$1; print $1} END {print "--------"; print s}' filename`

- Print every third line starting from the first line:

  ` awk 'NR%3==1' filename`
