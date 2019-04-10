# Linux jobs Command
-------------------
### Command Introduction (命令介绍)
> **bash, :, ., [, alias, bg, bind, break, builtin, caller, cd, command, compgen, complete, compopt, continue, declare, dirs, disown, echo, enable, eval, exec, exit, export,**
### Command Format and Options (命令格式和选项)
```
jobs: usage: jobs [-lnprs] [jobspec ...] or jobs -x command [args]
```
### Command Example (命令范例)
```

  jobs

  BASH builtin for viewing information about processes spawned by the current shell.

  - View jobs spawned by the current shell:
    jobs

  - List jobs and their process ids:
    jobs -l

  - Display information about jobs with changed status:
    jobs -n

  - Display process id of process group leader:
    jobs -p

  - Display running processes:
    jobs -r

  - Display stopped processes:
    jobs -s


```
