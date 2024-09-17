# Day 11 Lab - Troubleshooting Static Routes

## PC1 Command Prompt

### Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 192.168.3.1
```

Display all current TCP/IP network configuration values

```
ipconfig
```

Displays the full TCP/IP configuration for all adapters

```
ipconfig /all
```

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 192.168.1.254
```

## Router 1

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

View the routing table

```
#show ip route
```

Show running-config, limit output to ip route

```
#show running-config | include ip route
```

Disable a recursive static route

```
(config-if)#no ip route <destination-network> <netmask> <next-hop>
```

Configure a recursive static route

```
(config-if)#ip route <destination-network> <netmask> <next-hop>
```

## Router 2

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

View the routing table

```
#show ip route
```

Configure a directly connected static route

```
(config-if)#ip route <destination-network> <netmask> <exit-interface>
```

Show running-config, limit output to ip route

```
#show running-config | include ip route
```

Disable a directly connected static route

```
(config-if)#no ip route <destination-network> <netmask> <exit-interface>
```

## Router 3

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

Show running-config

```
#show running-config
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
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
