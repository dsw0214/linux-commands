# Linux pwd Command
### Command Introduction (命令介绍)
-------------------
> **pwd - print name of current/working directory**

### Command Format and Options (命令格式和选项)
```
#pwd: usage: pwd [-LP]
 -L, --logical
      use PWD from environment, even if it contains symlinks

-P, --physical
      avoid all symlinks

--help display this help and exit

--version
      output version information and exit

```
### Command Example (命令范例)
-------------------
**Print name of current/working directory.**

- Print the current directory:

  ` pwd`

- Print the current directory, and resolve all symlinks (i.e. show the "physical" path):

  ` pwd -P`
