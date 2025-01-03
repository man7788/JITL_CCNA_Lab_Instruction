# Day 38 Lab - DNS

# Step 1

Configure a recursive static route

```
(config)#ip route <destination-network> <netmask> <next-hop>
```

Send Internet Control Message Protocol (ICMP) echo Request messages

```
#ping 1.1.1.1
```

# Step 2

## PC

Config all PC's Default Gateway

- Gateway/DNS Static - 1.1.1.1

##

# Step 3

Configure the DNS server(s) to send DNS queries to

```
(config)#ip name-server <ip-address>
```

Create a manual name-to-IP mapping

```
(config)#ip host <hostname> <ip-address>
```

View all name-to-IP mappings

```
#show hosts
```

Send Internet Control Message Protocol (ICMP) echo Request messages

```
#ping PC1
```

# Step 4

## PC

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping youtube.com
```

##
