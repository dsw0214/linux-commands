# Linux locate Command
-------------------
### Command Introduction (命令介绍)
> ****
### Command Format and Options (命令格式和选项)
```
#locate --help
create.sh: line 20: locate: command not found
```
### Command Example (命令范例)
```

  locate

  Find filenames quickly.

  - Look for pattern in the database. Note: the database is recomputed periodically (usually weekly or daily):
    locate pattern

  - Look for a file by its exact filename (a pattern containing no globbing characters is interpreted as *pattern*):
    locate */filename

  - Recompute the database. You need to do it if you want to find recently added files:
    sudo updatedb


```
