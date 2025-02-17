# Day 38 Lab - DNS

# Step 1

Configure a recursive static route.

```
(config)# ip route <destination-network> <netmask> <next-hop>
```

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
# ping <targetname>
```

# Step 2

### PC's Config GUI > GLOBAL > Settings

#### Gateway/DNS IPv4 > Static

- Configure Default Gateway.

# Step 3

Configure the DNS server(s) to send DNS queries to.

```
(config)# ip name-server <ip-address>
```

Create a manual name-to-IP mapping.

```
(config)# ip host <hostname> <ip-address>
```

View all name-to-IP mappings.

```
# show hosts
```

Send Internet Control Message Protocol (ICMP) echo Request messages. 

```
# ping <targetname>
```

# Step 4

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```
