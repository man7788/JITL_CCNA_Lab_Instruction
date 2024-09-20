# Day 26 Lab - OSPF (Part 1)

## Step 2

Create/configure a loopback interface

```
interface loopback <number>
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

View interface Layer 1/2 information

```
#show interfaces [interface]
```

## Step 3

Create/configure an OSPF process

```
(config)#router ospf <process-id>
```

Activate OSPF on all interfaces

```
(config-router)#network 0.0.0.0 255.255.255.255 area <area>
```

Configure a passive interface

```
(config-router)#passive-interface <interface>
```

Activate OSPF on interfaces with an IP address in the specified range

```
(config-router)#network <ip-address> <wildcard-mask> area <area>
```

> Different ways to config OSPF

1. Exact IP address with /32 prefix
2. Network address of all interfaces e.g. IP address with /16 prefix
3. Network address of individual interfaces e.g. IP address with /31 subnet prefix

## Step 4

Advertise a default route to other routers

```
(config-router)#default-information originate
```

Configure a default route

```
(config)# ip route 0.0.0.0 0.0.0.0 <next-hop>
```

View information about router's active routing protocols

```
#show ip protocols
```

View the OSPF LSDB

```
#show ip ospf database
```

View OSPF neighbors and their status

```
#show ip ospf neighbor
```

View information about all OSPF interfaces/an OSPF interface

```
#show ip ospf interface <interface>
```

## Step 5

View the routing table

```
#show ip route
```
