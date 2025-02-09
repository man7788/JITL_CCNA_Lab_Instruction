# Day 24 Lab - Floating Static Routes

## Step 1

View the routing table.

```
# show ip route
```

Which dynamic routing protocol is Enterprise A using?

- OSPF

Which route will be used if PC1 tries to access SRV1?

- The OSPF route.

Which route will be used if PC1 tries to access remote server 1.1.1.1 over the Internet?

- The default route.

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

View a concise summary of interface IP addresses and status.

```
# show ip interface brief
```

## Step 2

Configure a floating static route.

```
(config)# ip route <destination-network> <netmask> <next-hop> <administrative-distance>
```

View the routing table.

```
# show ip route
```

## Step 3

Disable the interface.

```
(config-if)# shutdown
```

View the routing table.

```
# show ip route
```

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
> tracert <targetname>
```
