# Linux ping Command
### Command Introduction (命令介绍)
-------------------
> **ping - send ICMP ECHO_REQUEST to network hosts**

### Command Format and Options (命令格式和选项)
```
#ping --help
ping: invalid option -- '-'
Usage: ping [-aAbBdDfhLnOqrRUvV] [-c count] [-i interval] [-I interface]
            [-m mark] [-M pmtudisc_option] [-l preload] [-p pattern] [-Q tos]
            [-s packetsize] [-S sndbuf] [-t ttl] [-T timestamp_option]
            [-w deadline] [-W timeout] [hop1 ...] destination

```
### Command Example (命令范例)
-------------------
**Send ICMP ECHO_REQUEST packets to network hosts.** 

- Ping host:

  ` ping host`

- Ping a host only a specific number of times:

  ` ping -c count host`

- Ping host, specifying the interval in seconds between requests (default is 1 second):

  ` ping -i seconds host`

- Ping host without trying to lookup symbolic names for addresses:

  ` ping -n host`

- Ping host and ring the bell when a packet is received (if your terminal supports it):

  ` ping -a host`

- Also display a message if no response was received:

  ` ping -O host`



