# Day 53 Lab - GRE Tunnels

# Step 1

Create a new tunnel interface.

```
(config)# interface tunnel <number>
```

Configure the source address for the IP tunnel.

```
(config-if)# tunnel source {<ip-address> | <interface-name>}
```

Configure the destination address for the IP tunnel.

```
(config-if)# tunnel destination {<ip-address> | <host-name>}
```

Set the interfaces's IP address/netmask.

```
(config-if)# ip address <ip-address> <netmask>
```

View a concise summary of interface IP addresses and status.

```
# show ip interface brief
```

View the routing table.

```
# show ip route
```

Configure a recursive static route.

```
(config)# ip route <destination-network> <netmask> <next-hop>
```

Send Internet Control Message Protocol (ICMP) echo Request messages

```
# ping <targetname>
```

# Step 2

Create/configure an OSPF process.

```
(config)# router ospf <process-id>
```

Activate OSPF on interfaces with an IP address in the specified range.

```
(config-router)# network <ip-address> <wildcard-mask> area <area>
```

Configure a passive interface.

```
(config-router)# passive-interface <interface>
```

View the routing table.

```
# show ip route
```
##

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

