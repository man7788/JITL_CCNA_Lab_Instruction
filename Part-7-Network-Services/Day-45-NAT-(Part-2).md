# Day 45 Lab - NAT Part 2

# Step 1

Configure an inside interface

```
(config-if)#ip nat inside
```

Configure an outside interface

```
(config-if)#ip nat outside
```

Configure an ACE in a standard numbered ACL

```
(config)#access-list <number> {permit | deny} <src-ip> <wildcard>
```

Create a NAT pool

```
(config)#ip nat pool <pool-name> <start-ip> <end-ip> {prefix-length <length> | netmask <subnet-mask>}
```

Configure a dynamic NAT mapping of an ACL to a NAT pool

```
(config)#ip nat inside source list <acl> pool <pool-name>
```

# Step 2

## PCs

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping google.com
```

##

View the NAT translation table

```
#show ip nat translations
```

# Step 3

Clear the NAT translation table

```
#clear ip nat translation *
```

Show running-config, limit output to NAT

```
#show running-config | include nat
```

Configure a dynamic PAT mapping of an ACL to an interface IP address

```
(config)#ip nat inside source list interface <interface> [overload]
```

# Step 4

## PCs

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping google.com
```

##

View the NAT translation table

```
#show ip nat translations
```
