# Linux dig Command
-------------------
### Command Introduction (命令介绍)
> **dig - DNS lookup utility**
### Command Format and Options (命令格式和选项)
```
#dig --help
Invalid option: --help
Usage:  dig [@global-server] [domain] [q-type] [q-class] {q-opt}
            {global-d-opt} host [@local-server] {local-d-opt}
            [ host [@local-server] {local-d-opt} [...]]

Use "dig -h" (or "dig -h | more") for complete list of options
```
### Command Example (命令范例)
```

  dig

  DNS Lookup utility.

  - Lookup the IP(s) associated with a hostname (A records):
    dig +short hostname.com

  - Lookup the mail server(s) associated with a given domain name (MX record):
    dig +short hostname.com MX

  - Get all types of records for a given domain name:
    dig hostname.com ANY

  - Specify an alternate DNS server to query:
    dig @8.8.8.8 hostname.com

  - Perform a reverse DNS lookup on an IP address (PTR record):
    dig -x 8.8.8.8

  - Find authoritative name servers for the zone and display SOA records:
    dig +nssearch hostname.com

  - Perform iterative queries and display the entire trace path to resolve a domain name:
    dig +trace hostname.com


```
