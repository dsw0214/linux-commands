# Linux chkconfig Command
-------------------
### Command Introduction (命令介绍)
> **chkconfig - updates and queries runlevel information for system services**
### Command Format and Options (命令格式和选项)
```
#chkconfig --help
chkconfig version 1.7.4 - Copyright (C) 1997-2000 Red Hat, Inc.
This may be freely redistributed under the terms of the GNU Public License.

usage:   chkconfig [--list] [--type <type>] [name]
         chkconfig --add <name>
         chkconfig --del <name>
         chkconfig --override <name>
         chkconfig [--level <levels>] [--type <type>] <name> <on|off|reset|resetpriorities>
```
### Command Example (命令范例)
```

  chkconfig

  Manage the runlevel of services on CentOS 6.

  - List services with runlevel:
    chkconfig --list

  - Show a service's runlevel:
    chkconfig --list ntpd

  - Enable service at boot:
    chkconfig sshd on

  - Enable service at boot for runlevels 2, 3, 4, and 5:
    chkconfig --level 2345 sshd on

  - Disable service at boot:
    chkconfig ntpd off

  - Disable service at boot for runlevel 3:
    chkconfig --level 3 ntpd off


```
