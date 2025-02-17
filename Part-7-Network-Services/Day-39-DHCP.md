# Day 39 Lab - DHCP

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

Set the pool's DNS server.

```
(dhcp-config)# dns-server <ip-address>
```

Set the pool's domain name.

```
(dhcp-config)# domain-name <domain-name>
```

Set the pool's default gateway.

```
(dhcp-config)# default-router <ip-address>
```

View the running-config.

```
# show running-config | section dhcp
```

# Step 2

Configure the interface as a DHCP client.

```
(config-if)# ip address dhcp
```

Enable the interface.

```
(config-if)# no shutdown
```

# Step 3

Configure the interface as a DHCP relay agent.

```
(config-if)# ip helper-address <ip-address>
```

# Step 4

### PC's Command Prompt

Renew DHCP configuration for all adapters.

```
> ipconfig /renew
```
