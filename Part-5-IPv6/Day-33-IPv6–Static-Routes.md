# Day 33 Lab - IPv6 Static Routes

# Step 1

Enable IPv6 routing

```
(config)#ipv6 unicast-routing
```

# Step 2

1. Config PC's IPv6 Default Gateway (Auto)
2. Config PC's Interface IPv6 Address (Auto)

# Step 3

Configure a fully specified static route

```
(config)#ipv6 route <destination-prefix> <exit-interface> <next-hop> [ad]
```

View a concise summary of interface IPv6 addresses and status

```
#show ipv6 interface brief
```

View the IPv6 routing table

```
#show ipv6 route
```

Show running-config, limit output to IPv6 route

```
#show running-config | include ipv6 route
```

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 2001:db8:0:3:240:bff:fe69:9b18
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
tracert 2001:db8:0:3:240:bff:fe69:9b18
```

### Delete the cable between R1 and R3

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
tracert 2001:db8:0:3:240:bff:fe69:9b18
```
