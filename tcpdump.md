# Linux tcpdump Command
-------------------
### Command Introduction (命令介绍)
> **tcpdump - dump traffic on a network**
### Command Format and Options (命令格式和选项)
```
#tcpdump --help
tcpdump version 4.9.2
libpcap version 1.5.3
OpenSSL 1.0.2k-fips  26 Jan 2017
Usage: tcpdump [-aAbdDefhHIJKlLnNOpqStuUvxX#] [ -B size ] [ -c count ]
		[ -C file_size ] [ -E algo:secret ] [ -F file ] [ -G seconds ]
		[ -i interface ] [ -j tstamptype ] [ -M secret ] [ --number ]
		[ -Q|-P in|out|inout ]
		[ -r file ] [ -s snaplen ] [ --time-stamp-precision precision ]
		[ --immediate-mode ] [ -T type ] [ --version ] [ -V file ]
		[ -w file ] [ -W filecount ] [ -y datalinktype ] [ -z postrotate-command ]
		[ -Z user ] [ expression ]
```
### Command Example (命令范例)
```

  tcpdump

  Dump traffic on a network.

  - List available network interfaces:
    tcpdump -D

  - Capture the traffic of a specific interface:
    tcpdump -i eth0

  - Capture all TCP traffic showing contents (ASCII) in console:
    tcpdump -A tcp

  - Capture the traffic from or to a host:
    tcpdump host www.example.com

  - Capture the traffic from a specific interface, source, destination and destination port:
    tcpdump -i eth0 src 192.168.1.1 and dst 192.168.1.2 and dst port 80

  - Capture the traffic of a network:
    tcpdump net 192.168.1.0/24

  - Capture all traffic except traffic over port 22 and save to a dump file:
    tcpdump -w dumpfile.pcap not port 22

  - Read from a given dump file:
    tcpdump -r dumpfile.pcap


```
