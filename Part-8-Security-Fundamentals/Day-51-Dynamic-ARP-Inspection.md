# Day 51 Lab - Dynamic ARP Inspection

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

Disable option 82 insertion.

```
(config)# no ip dhcp snooping information option
```

Configure the port as a DHCP Snooping trusted port.

```
(config-if)# ip dhcp snooping trust
```

# Step 3

Enable DAI on the specified VLANs.

```
(config)# ip arp inspection vlan <vlans>
```

Enable optional DAI checks.

```
(config)# ip arp inspection validate {[src-mac] [dst-mac] [ip]}
```

Configure the port as a DAI trusted port.

```
(config-if)# ip arp inspection trust
```

View the running-config.

```
# show running-config
```

View DAI interface status and settings.

```
# show ip arp inspection interfaces
```

##

### PC's Config GUI > GLOBAL > Settings

#### Gateway/DNS IPv4 > DHCP

- Configure Default Gateway.

### PC's Command Prompt

Display all current TCP/IP network configuration values.

```
> ipconfig
```

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```
