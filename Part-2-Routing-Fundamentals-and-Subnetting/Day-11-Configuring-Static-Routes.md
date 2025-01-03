# Day 11 Lab - Configuring Static Routes

## Step 1

### PC

1. Config all PC's Default Gateway
2. Config all PC's Interface IP Address
3. Config all PC's Interface Subnet Mask

### Router

Set the device's hostname

```
(config)#hostname <hostname>
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

Set the interfaces's description

```
(config-if)#description <description>
```

Enable/disable the interface

```
(config-if)#[no] shutdown
```

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

## Step 2

Configure a recursive static route

```
(config)#ip route <destination-network> <netmask> <next-hop>
```

Configure a directly connected static route

```
(config)#ip route <destination-network> <netmask> <exit-interface>
```

View the routing table

```
#show ip route
```

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 192.168.3.1
```
