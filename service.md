# Linux service Command
### Command Introduction (命令介绍)
-------------------
> ** service - run a System V init script **

### Command Format and Options (命令格式和选项)
```
#service --help
Usage: service < option > | --status-all | [ service_name [ command | --full-restart ] ]
```
### Command Example (命令范例)
-------------------
**
Manage services by running init scripts.
The full script path should be omitted (/etc/init.d/ is assumed).
**

- Start/Stop/Restart/Reload service (start/stop should always be available):

  ` service init_script start|stop|restart|reload`

- Do a full restart (runs script twice with start and stop):

  ` service init_script --full-restart`

- Show the current status of a service:

  ` service init_script status`

- List the status of all services:

  ` service --status-all`
