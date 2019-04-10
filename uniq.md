# Linux uniq Command
-------------------
### Command Introduction (命令介绍)
> **uniq - report or omit repeated lines**
### Command Format and Options (命令格式和选项)
```
#uniq --help
Usage: uniq [OPTION]... [INPUT [OUTPUT]]
Filter adjacent matching lines from INPUT (or standard input),
writing to OUTPUT (or standard output).

With no options, matching lines are merged to the first occurrence.

Mandatory arguments to long options are mandatory for short options too.
  -c, --count           prefix lines by the number of occurrences
  -d, --repeated        only print duplicate lines, one for each group
  -D, --all-repeated[=METHOD]  print all duplicate lines
                          groups can be delimited with an empty line
                          METHOD={none(default),prepend,separate}
  -f, --skip-fields=N   avoid comparing the first N fields
      --group[=METHOD]  show all items, separating groups with an empty line
                          METHOD={separate(default),prepend,append,both}
  -i, --ignore-case     ignore differences in case when comparing
  -s, --skip-chars=N    avoid comparing the first N characters
  -u, --unique          only print unique lines
  -z, --zero-terminated  end lines with 0 byte, not newline
  -w, --check-chars=N   compare no more than N characters in lines
      --help     display this help and exit
      --version  output version information and exit

A field is a run of blanks (usually spaces and/or TABs), then non-blank
characters.  Fields are skipped before chars.

Note: 'uniq' does not detect repeated lines unless they are adjacent.
You may want to sort the input first, or use 'sort -u' without 'uniq'.
Also, comparisons honor the rules specified by 'LC_COLLATE'.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
For complete documentation, run: info coreutils 'uniq invocation'
```
### Command Example (命令范例)
```

  uniq

  Output the unique lines from the given input or file.
  Since it does not detect repeated lines unless they are adjacent, we need to sort them first.

  - Display each line once:
    sort file | uniq

  - Display only unique lines:
    sort file | uniq -u

  - Display only duplicate lines:
    sort file | uniq -d

  - Display number of occurrences of each line along with that line:
    sort file | uniq -c

  - Display number of occurrences of each line, sorted by the most frequent:
    sort file | uniq -c | sort -nr


```
