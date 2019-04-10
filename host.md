# Linux host Command
-------------------
### Command Introduction (命令介绍)
> **host - DNS lookup utility**
### Command Format and Options (命令格式和选项)
```
#host --help
host: illegal option -- -
Usage: host [-aCdlriTwv] [-c class] [-N ndots] [-t type] [-W time]
            [-R number] [-m flag] hostname [server]
       -a is equivalent to -v -t ANY
       -c specifies query class for non-IN data
       -C compares SOA records on authoritative nameservers
       -d is equivalent to -v
       -l lists all hosts in a domain, using AXFR
       -i IP6.INT reverse lookups
       -N changes the number of dots allowed before root lookup is done
       -r disables recursive processing
       -R specifies number of retries for UDP packets
       -s a SERVFAIL response should stop query
       -t specifies the query type
       -T enables TCP/IP mode
       -v enables verbose output
       -w specifies to wait forever for a reply
       -W specifies how long to wait for a reply
       -4 use IPv4 query transport only
       -6 use IPv6 query transport only
       -m set memory debugging flag (trace|record|usage)
```
### Command Example (命令范例)
```

  host

  Lookup Domain Name Server.

  - Lookup A, AAAA, and MX records of a domain:
    host domain

  - Lookup a field (CNAME, TXT,...) of a domain:
    host -t field domain

  - Reverse lookup an IP:
    host ip_address

  - Specify an alternate DNS server to query:
    host domain 8.8.8.8


```
