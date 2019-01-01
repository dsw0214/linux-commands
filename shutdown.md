# Linux shutdown Command
### Command Introduction (命令介绍)
-------------------
> ** shutdown - Halt, power-off or reboot the machine **

### Command Format and Options (命令格式和选项)
```
#shutdown --help
shutdown [OPTIONS...] [TIME] [WALL...]

Shut down the system.

     --help      Show this help
  -H --halt      Halt the machine
  -P --poweroff  Power-off the machine
  -r --reboot    Reboot the machine
  -h             Equivalent to --poweroff, overridden by --halt
  -k             Don't halt/power-off/reboot, just send warnings
     --no-wall   Don't send wall message before halt/power-off/reboot
  -c             Cancel a pending shutdown
```
### Command Example (命令范例)
-------------------
** Shutdown and reboot the system. **

- Power off (halt) immediately:

  ` shutdown -h now`

- Reboot immediately:

  ` shutdown -r now`

- Reboot in 5 minutes:

  ` shutdown -r +5 &`

- Shutdown at 1:00 pm (Uses 24h clock):

  ` shutdown -h 13:00`

- Cancel a pending shutdown/reboot operation:

  ` shutdown -c`
