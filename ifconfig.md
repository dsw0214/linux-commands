# Linux ifconfig Command
### Command Introduction (命令介绍)
-------------------
> ** ifconfig - configure a network interface **

### Command Format and Options (命令格式和选项)
```
#ifconfig --help
Usage:
  ifconfig [-a] [-v] [-s] <interface> [[<AF>] <address>]
  [add <address>[/<prefixlen>]]
  [del <address>[/<prefixlen>]]
  [[-]broadcast [<address>]]  [[-]pointopoint [<address>]]
  [netmask <address>]  [dstaddr <address>]  [tunnel <address>]
  [outfill <NN>] [keepalive <NN>]
  [hw <HW> <address>]  [mtu <NN>]
  [[-]trailers]  [[-]arp]  [[-]allmulti]
  [multicast]  [[-]promisc]
  [mem_start <NN>]  [io_addr <NN>]  [irq <NN>]  [media <type>]
  [txqueuelen <NN>]
  [[-]dynamic]
  [up|down] ...

  <HW>=Hardware Type.
  List of possible hardware types:
    loop (Local Loopback) slip (Serial Line IP) cslip (VJ Serial Line IP) 
    slip6 (6-bit Serial Line IP) cslip6 (VJ 6-bit Serial Line IP) adaptive (Adaptive Serial Line IP) 
    ash (Ash) ether (Ethernet) ax25 (AMPR AX.25) 
    netrom (AMPR NET/ROM) rose (AMPR ROSE) tunnel (IPIP Tunnel) 
    ppp (Point-to-Point Protocol) hdlc ((Cisco)-HDLC) lapb (LAPB) 
    arcnet (ARCnet) dlci (Frame Relay DLCI) frad (Frame Relay Access Device) 
    sit (IPv6-in-IPv4) fddi (Fiber Distributed Data Interface) hippi (HIPPI) 
    irda (IrLAP) ec (Econet) x25 (generic X.25) 
    infiniband (InfiniBand) eui64 (Generic EUI-64) 
  <AF>=Address family. Default: inet
  List of possible address families:
    unix (UNIX Domain) inet (DARPA Internet) inet6 (IPv6) 
    ax25 (AMPR AX.25) netrom (AMPR NET/ROM) rose (AMPR ROSE) 
    ipx (Novell IPX) ddp (Appletalk DDP) ec (Econet) 
    ash (Ash) x25 (CCITT X.25) 

```
### Command Example (命令范例)
-------------------
** Network Interface Configurator. **

- View network settings of an ethernet adapter:

  ` ifconfig eth0`

- Display details of all interfaces, including disabled interfaces:

  ` ifconfig -a`

- Disable eth0 interface:

  ` ifconfig eth0 down`

- Enable eth0 interface:

  ` ifconfig eth0 up`

- Assign IP address to eth0 interface:

  ` ifconfig eth0 ip_address`
