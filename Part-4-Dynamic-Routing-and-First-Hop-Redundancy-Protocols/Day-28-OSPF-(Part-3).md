# Day 28 Lab - OSPF (Part 3)

## Step 1

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

Identify which side is DCE / DTE

```
#show controllers <interface-id>
```

Configure the clock rate on the DCE side

```
(config-if)#clock rate <bps>
```

Enable the interface

```
(config-if)#no shutdown
```

View information about router's active routing protocols

```
#show ip protocols
```

Activate OSPF on the interface

```
(config-if)#ip ospf <process-id> area <area>
```

View information about an OSPF interface

```
#show ip ospf interface <interface>
```

View the routing table

```
#show ip route
```

## Step 2

View OSPF neighbors and their status

```
#show ip ospf neighbor
```

View the routing table

```
#show ip route
```

View information about an OSPF interface

```
#show ip ospf interface <interface>
```

Set the interface's OSPF network type

```
(config-if)#no ip ospf network point-to-point
```

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 10.0.2.1
```

## Step 3

View OSPF neighbors and their status

```
#show ip ospf neighbor
```

View information about an OSPF interface

```
#show ip ospf interface <interface>
```

Set the interfaces's hello timer

```
(config-if)#no ip ospf hello-interval
```

Set the interfaces's dead timer

```
(config-if)#no ip ospf dead-interval
```

## Step 4

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 8.8.8.8
```

View the running-config

```
#show running-config | section ospf
```

Configure a default route

```
(config)# ip route 0.0.0.0 0.0.0.0 <next-hop>
```

View the routing table

```
#show ip route
```

## Step 5

View the OSPF LSDB

```
#show ip ospf database
```
