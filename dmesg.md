# Linux dmesg Command
-------------------
### Command Introduction (命令介绍)
> **dmesg - print or control the kernel ring buffer**
### Command Format and Options (命令格式和选项)
```
#dmesg --help

Usage:
 dmesg [options]

Options:
 -C, --clear                 clear the kernel ring buffer
 -c, --read-clear            read and clear all messages
 -D, --console-off           disable printing messages to console
 -d, --show-delta            show time delta between printed messages
 -e, --reltime               show local time and time delta in readable format
 -E, --console-on            enable printing messages to console
 -F, --file <file>           use the file instead of the kernel log buffer
 -f, --facility <list>       restrict output to defined facilities
 -H, --human                 human readable output
 -k, --kernel                display kernel messages
 -L, --color                 colorize messages
 -l, --level <list>          restrict output to defined levels
 -n, --console-level <level> set level of messages printed to console
 -P, --nopager               do not pipe output into a pager
 -r, --raw                   print the raw message buffer
 -S, --syslog                force to use syslog(2) rather than /dev/kmsg
 -s, --buffer-size <size>    buffer size to query the kernel ring buffer
 -T, --ctime                 show human readable timestamp (could be 
                               inaccurate if you have used SUSPEND/RESUME)
 -t, --notime                don't print messages timestamp
 -u, --userspace             display userspace messages
 -w, --follow                wait for new messages
 -x, --decode                decode facility and level to readable string

 -h, --help     display this help and exit
 -V, --version  output version information and exit

Supported log facilities:
    kern - kernel messages
    user - random user-level messages
    mail - mail system
  daemon - system daemons
    auth - security/authorization messages
  syslog - messages generated internally by syslogd
     lpr - line printer subsystem
    news - network news subsystem

Supported log levels (priorities):
   emerg - system is unusable
   alert - action must be taken immediately
    crit - critical conditions
     err - error conditions
    warn - warning conditions
  notice - normal but significant condition
    info - informational
   debug - debug-level messages


For more details see dmesg(q).
```
### Command Example (命令范例)
```

  dmesg

  Write the kernel messages to standard output.

  - Show kernel messages:
    dmesg

  - Show kernel error messages:
    dmesg --level err

  - Show kernel messages and keep reading new ones, similar to tail -f (available in kernels 3.5.0 and newer):
    dmesg -w

  - Show how much physical memory is available on this system:
    dmesg | grep -i memory

  - Show kernel messages 1 page at a time:
    dmesg | less

  - Show kernel messages with a timestamp (available in kernels 3.5.0 and newer):
    dmesg -T

  - Show kernel messages in human-readable form (available in kernels 3.5.0 and newer):
    dmesg -H

  - Colorize output (available in kernels 3.5.0 and newer):
    dmesg -L


```
