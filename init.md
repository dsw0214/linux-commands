# Linux init Command
-------------------
### Command Introduction (命令介绍)
> **systemd, init - systemd system and service manager**
### Command Format and Options (命令格式和选项)
```
#init --help
init [OPTIONS...] {COMMAND}

Send control commands to the init daemon.

     --help      Show this help
     --no-wall   Don't send wall message before halt/power-off/reboot

Commands:
  0              Power-off the machine
  6              Reboot the machine
  2, 3, 4, 5     Start runlevelX.target unit
  1, s, S        Enter rescue mode
  q, Q           Reload init daemon configuration
  u, U           Reexecute init daemon
```
### Command Example (命令范例)
```
```
