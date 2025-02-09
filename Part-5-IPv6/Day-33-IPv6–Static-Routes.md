# Day 33 Lab - IPv6 Static Routes

# Step 1

Enable IPv6 routing.

```
(config)# ipv6 unicast-routing
```

# Step 2

### PC's Config GUI > GLOBAL > Settings

#### Gateway/DNS IPv6 > Automatic

- Configure Default Gateway.

### PC's Config GUI > INTERFACE > FastEthernet0

#### IPv6 Configuration > Automatic

- Configure IP Address/Prefix-Length.

# Step 3

Configure a fully specified static route.

```
(config)# ipv6 route <destination-prefix> <exit-interface> <next-hop> [ad]
```

View a concise summary of interface IPv6 addresses and status.

```
# show ipv6 interface brief
```

View the IPv6 routing table.

```
# show ipv6 route
```

View the running-config, limit output to IPv6 route.

```
# show running-config | include ipv6 route
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

### Delete the cable between R1 and R3

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
> tracert <targetname>
```
