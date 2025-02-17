# Day 49 Lab - Port Security

# Step 1

Enable aging, and set the aging time for secure MAC addresses learned on the port.

```
(config-if)# switchport port-security aging time <minutes>
```

Show interface switchport information.

```
# show interfaces <interface-id> switchport
```

Manually configure access mode.

```
(config-if)# switchport mode access
```

Enable Port Security on the port.

```
(config-if)# switchport port-security
```

View Port Security settings for a port.

```
# show port-security interface <interface>
```

Set the Port Security violation mode of the port.

```
(config-if)# switchport port-security violation {shutdown | restrict | protect}
```

Limit the maximum number of MAC addresses that can be learned on the port.

```
(config-if)# switchport port-security maximum <number>
```

Enable sticky secure MAC address learning.

```
(config-if)# switchport port-security mac-address sticky
```

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

##

View the running-config.

```
# show running-config
```

View secure MAC addresses.

```
# show mac address-table secure
```

View a list of Port Security-enabled ports.

```
# show port-security
```

# Step 2

Configure a switch virtual interface (SVI).

```
(config)# interface vlan <vlan-id>
```

Set the interfaces's IP address/netmask.

```
(config-if)# ip address <ip-address> <netmask>
```

Enable the interface.

```
(config-if)# no shutdown
```

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
# ping <targetname>
```

View Port Security settings for a port.

```
# show port-security interface <interface>
```

##

### PC's Config > INTERFACE > FastEthernet0

- Change MAC address to 0001.0001.000A


### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

##
