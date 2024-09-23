# Day 31 Lab - IPv6 Configuration (Part 1)

## Step 1

Enable IPv6 routing

```
(config)#ipv6 unicast-routing
```

## Step 2

Configure an IPv6 address

```
(config-if)#ipv6 address <address/prefix-length>
```

## Step 3

View a concise summary of interface IPv6 addresses and status

```
#show ipv6 interface brief
```

# Step 4

2. Config PC's IPv6 Default Gateway
1. Config PC's Interface IPv6 Address

# Step 5

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 192.168.x.2
```

```
2001:db8:0:x::2
```
