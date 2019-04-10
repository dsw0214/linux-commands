# Linux route Command
-------------------
### Command Introduction (命令介绍)
> **route - show / manipulate the IP routing table**
### Command Format and Options (命令格式和选项)
```
#route --help
Usage: route [-nNvee] [-FC] [<AF>]           List kernel routing tables
       route [-v] [-FC] {add|del|flush} ...  Modify routing table for AF.

       route {-h|--help} [<AF>]              Detailed usage syntax for specified AF.
       route {-V|--version}                  Display version/author and exit.

        -v, --verbose            be verbose
        -n, --numeric            don't resolve names
        -e, --extend             display other/more information
        -F, --fib                display Forwarding Information Base (default)
        -C, --cache              display routing cache instead of FIB

  <AF>=Use -4, -6, '-A <af>' or '--<af>'; default: inet
  List of possible address families (which support routing):
    inet (DARPA Internet) inet6 (IPv6) ax25 (AMPR AX.25) 
    netrom (AMPR NET/ROM) ipx (Novell IPX) ddp (Appletalk DDP) 
    x25 (CCITT X.25) 
```
### Command Example (命令范例)
```

  route

  Use route cmd to set the route table .

  - Display the information of route table:
    route -n

  - Add route rule:
    sudo route add -net ip_address netmask netmask_address gw gw_address

  - Delete route rule:
    sudo route del -net ip_address netmask netmask_address dev gw_address


```
