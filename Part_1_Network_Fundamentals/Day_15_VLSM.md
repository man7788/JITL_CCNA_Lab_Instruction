# Day 15 Lab - VLSM

### Router

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

Enable the interface

```
(config-if)#no shutdown
```

View detailed Layer 3 information about interfaces

```
#show ip interfaces [interface]
```

Configure a recursive static route

```
(config-if)#ip route <destination-network> <netmask> <next-hop>
```

View the routing table

```
#show ip route
```

### PC

- Config all PC's Default Gateway

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 192.168.5.xxx
```

## LAN 2

### /25

- Network Address: 192.168.5.0
- Broadcast Address: 192.168.5.127
- First Usable Address: 192.168.5.1
- Last Usable Address: 192.168.5.126
- Usable Address: 126

## LAN 1

### /26

- Network Address: 192.168.5.128
- Broadcast Address: 192.168.5.191
- First Usable Address: 192.168.5.129
- Last Usable Address: 192.168.5.190
- Usable Address: 62

## LAN 3

### /28

- Network Address: 192.168.5.192
- Broadcast Address: 192.168.5.207
- First Usable Address: 192.168.5.193
- Last Usable Address: 192.168.5.206
- Usable Address: 14

## LAN 4

### /28

- Network Address: 192.168.5.208
- Broadcast Address: 192.168.5.223
- First Usable Address: 192.168.5.209
- Last Usable Address: 192.168.5.222
- Usable Address: 14

## Point-to-Point

### /30

- Network Address: 192.168.5.224
- Broadcast Address: 192.168.5.227
- First Usable Address: 192.168.5.225
- Last Usable Address: 192.168.5.226
- Usable Address: 2
