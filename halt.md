# Linux halt Command
-------------------
### Command Introduction (命令介绍)
> **halt, poweroff, reboot - Halt, power-off or reboot the machine**
### Command Format and Options (命令格式和选项)
```
#halt --help
halt [OPTIONS...]

Halt the system.

     --help      Show this help
     --halt      Halt the machine
  -p --poweroff  Switch off the machine
     --reboot    Reboot the machine
  -f --force     Force immediate halt/power-off/reboot
  -w --wtmp-only Don't halt/power-off/reboot, just write wtmp record
  -d --no-wtmp   Don't write wtmp record
     --no-wall   Don't send wall message before halt/power-off/reboot
```
### Command Example (命令范例)
```

  halt

  Power off or reboot the machine.

  - Power the machine off:
    halt

  - Reboot the machine:
    halt --reboot


```
