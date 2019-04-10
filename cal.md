# Linux cal Command
-------------------
### Command Introduction (命令介绍)
> **cal - display a calendar**
### Command Format and Options (命令格式和选项)
```
#cal --help

Usage:
 cal [options] [[[day] month] year]

Options:
 -1, --one        show only current month (default)
 -3, --three      show previous, current and next month
 -s, --sunday     Sunday as first day of week
 -m, --monday     Monday as first day of week
 -j, --julian     output Julian dates
 -y, --year       show whole current year
 -V, --version    display version information and exit
 -h, --help       display this help text and exit

```
### Command Example (命令范例)
```

  cal

  Prints calendar information, with the current day highlighted.

  - Display a calendar for the current month:
    cal

  - Display previous, current and next month:
    cal -3

  - Use monday as the first day of the week:
    cal --monday

  - Display a calendar for a specific year (4 digits):
    cal year

  - Display a calendar for a specific month and year:
    cal month year


```
