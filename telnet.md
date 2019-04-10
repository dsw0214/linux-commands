# Linux telnet Command
-------------------
### Command Introduction (命令介绍)
> **SYNOPSIS**
### Command Format and Options (命令格式和选项)
```
Usage: telnet [-4] [-6] [-8] [-E] [-L] [-S tos] [-a] [-c] [-d] [-e char] [-l user]
```
### Command Example (命令范例)
```

  telnet

  Connect to a specified port of a host using the telnet protocol.

  - Telnet to the default port of a host:
    telnet host

  - Telnet to a specific port of a host:
    telnet ip_address port

  - Exit a telnet session:
    quit

  - Emit the default escape character combination for terminating the session:
    Ctrl + ]

  - Start telnet with "x" as the session termination character:
    telnet -e x ip_address port


```
