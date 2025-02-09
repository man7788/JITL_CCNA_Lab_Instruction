# Day 31 Lab - IPv6 Configuration (Part 1)

## Step 1

Enable IPv6 routing.

```
(config)# ipv6 unicast-routing
```

## Step 2

Configure an IPv6 address.

```
(config-if)# ipv6 address <address/prefix-length>
```

## Step 3

View a concise summary of interface IPv6 addresses and status.

```
# show ipv6 interface brief
```

# Step 4

### PC's Config GUI > GLOBAL > Settings

#### Gateway/DNS IPv6 > Static

- Configure Default Gateway.

### PC's Config GUI > INTERFACE > FastEthernet0

#### IPv6 Configuration > Static

- Configure IP Address/Prefix-Length.

# Step 5

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname> 
```
