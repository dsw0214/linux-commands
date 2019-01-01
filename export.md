# Linux export Command
### Command Introduction (命令介绍)
-------------------
> **export - Set a new environment variable**

### Command Format and Options (命令格式和选项)
```
#export 
export: usage: export [-fn] [name[=value] ...] or export -p
```
### Command Example (命令范例)
-------------------
**Command to mark shell variables in the current environment to be exported with any newly forked child processes.**

- Set a new environment variable:

  ` export VARIABLE=value`

- Remove an environment variable:

  ` export -n VARIABLE`

- Mark a shell function for export:

  ` export -f FUNCTION_NAME`

- Append something to the PATH variable:

  ` export PATH=$PATH:path/to/append`
