# Day 11 Lab - Troubleshooting Static Routes

## PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

Display all current TCP/IP network configuration values.

```
> ipconfig
```

Displays the full TCP/IP configuration for all adapters.

```
> ipconfig /all
```

## Router 1

View a concise summary of interface IP addresses and status.

```
# show ip interface brief
```

View the routing table.

```
# show ip route
```

View the running-config, limit output to ip route.

```
# show running-config | include ip route
```

Delete a recursive static route.

```
(config-if)# no ip route <destination-network> <netmask> <next-hop>
```

Configure a recursive static route.

```
(config)# ip route <destination-network> <netmask> <next-hop>
```

## Router 2

View a concise summary of interface IP addresses and status.

```
# show ip interface brief
```

View the routing table.

```
# show ip route
```

Configure a directly connected static route.

```
(config)# ip route <destination-network> <netmask> <exit-interface>
```

View the running-config, limit output to ip route.

```
# show running-config | include ip route
```

Delete a directly connected static route.

```
(config)# no ip route <destination-network> <netmask> <exit-interface>
```

## Router 3

View a concise summary of interface IP addresses and status.

```
# show ip interface brief
```

View the running-config.

```
# show running-config
```

Set the interfaces's IP address/netmask.

```
(config-if)# ip address <ip-address> <netmask>
```

View the routing table.

```
# show ip route
```
