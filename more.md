# Linux more Command
-------------------
### Command Introduction (命令介绍)
> **more - file perusal filter for crt viewing**
### Command Format and Options (命令格式和选项)
```
#more --help
more: unknown option -help
Usage: more [options] file...

Options:
  -d        display help instead of ring bell
  -f        count logical, rather than screen lines
  -l        suppress pause after form feed
  -p        do not scroll, clean screen and display text
  -c        do not scroll, display text and clean line ends
  -u        suppress underlining
  -s        squeeze multiple blank lines into one
  -NUM      specify the number of lines per screenful
  +NUM      display file beginning from line number NUM
  +/STRING  display file beginning from search string match
  -V        output version information and exit
```
### Command Example (命令范例)
```

  more

  Open a file for interactive reading, allowing scrolling and search (in forward direction only).

  - Open a file:
    more source_file

  - Page down:
    <Space>

  - Search for a string (press n to go to the next match):
    /something

  - Exit:
    q


See also: n, q


```
