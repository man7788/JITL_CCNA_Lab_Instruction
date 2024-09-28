# Day 34 Lab - Standard ACLs

## Step 1

Create/configure an OSPF process

```
(config)#router ospf <process-id>
```

Activate OSPF on interfaces with an IP address in the specified range

```
(config-router)#network <ip-address> <wildcard-mask> area <area>
```

View information about all OSPF interfaces/an OSPF interface

```
#show ip ospf interface
```

View OSPF neighbors and their status

```
#show ip ospf neighbor
```

View the routing table

```
#show ip route
```

## Step 2

Configure a standard named ACL

```
(config)#ip access-list standard <name>
```

Configure an ACE in the standard named ACL

```
(config-std-nacl)#{permit | deny} <src-ip> <wildcard>
```

Configure an ACE to all source IP addresses in the standard named ACL

```
(config-std-nacl)#{permit | deny} any
```

Apply an ACL to an interface

```
(config-if)#ip access-group <acl> {in | out}

```

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping <ip-address>
```

View all ACLs

```
#show access-lists
```

Configure an ACE in a standard numbered ACL

```
(config)#access-list <number> {permit | deny} <src-ip> <wildcard>
```

Configure an ACE to all source IP addresses in the standard numbered ACL

```
(config)#access-list <number> any
```

### PC's Command Prompt

Specifies ping continue sending echo Request messages to the destination until interrupted.

```
ping -t <ip-address>
```
