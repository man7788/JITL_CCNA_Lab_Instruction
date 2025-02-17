# Day 50 Lab - DHCP Snooping

# Step 1

Specify a range of addresses that the device won't lease to DHCP clients.

```
(config)# ip dhcp excluded-address <low-ip> <high-ip>
```

Create/configure a DHCP pool.

```
(config)# ip dhcp pool <name>
```

Set the range of IP addresses to lease to clients.

```
(dhcp-config)# network <address> {</prefix-length | <netmask>}
```

Set the pool's default gateway.

```
(dhcp-config)# default-router <ip-address>
```

# Step 2

Enable DHCP Snooping.

```
(config)# ip dhcp snooping
```

Activate DHCP Snooping VLANs.

```
(config)# ip dhcp snooping vlan <vlans>
```

Configure the port as a DHCP Snooping trusted port.

```
(config-if)# ip dhcp snooping trust
```

# Step 3

### PC's Command Prompt

Renew DHCP configuration for all adapters.

```
> ipconfig /renew
```

# Step 4

Disable option 82 insertion.

```
(config)# no ip dhcp snooping information option
```
