# Linux mpstat Command
-------------------
### Command Introduction (命令介绍)
> ****
### Command Format and Options (命令格式和选项)
```
#mpstat --help
mpstat [-P {cpu|ALL}] [internal [count]]
```
### Command Example (命令范例)
```

  mpstat

  Report CPU statistics.

  - Display CPU statistics every 2 seconds:
    mpstat 2

  - Display 5 reports, one by one, at 2 second intervals:
    mpstat 2 5

  - Display 5 reports, one by one, from a given processor, at 2 second intervals:
    mpstat -P 0 2 5


```
