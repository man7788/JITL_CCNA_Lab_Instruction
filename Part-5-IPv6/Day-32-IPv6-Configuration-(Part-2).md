# Day 32 Lab - IPv6 Configuration (Part 2)

## Step 1

View interface Layer 1/2 information

```
#show interfaces [interface]
```

Enable IPv6 routing

```
(config)#ipv6 unicast-routing
```

Configure an IPv6 address, using EUI-64 to generate the host portion

```
(config-if)#ipv6 address <prefix/prefix-length> eui-64
```

View a concise summary of interface IPv6 addresses and status

```
#show ipv6 interface brief
```

## Step 2

1. Config PC's IPv6 Default Gateway
2. Config PC's Interface IPv6 Address

## Step 3

Enable IPv6 on the interface without configuring an IPv6 address

```
(config-if)#ipv6 enable
```

View a concise summary of interface IPv6 addresses and status

```
#show ipv6 interface brief
```

## Step 4

Configure a fully specified static route

```
(config)#ipv6 route <destination-prefix> <exit-interface> <next-hop>
```

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 2001:db8:0:1::2
```
