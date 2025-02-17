# Day 46 Lab - Voice VLANs

# Step 1

Manually configure access mode.

```
(config-if)# switchport mode access
```

Set the port's access VLAN.

```
(config-if)# switchport access vlan <vlan-id>
```

Configure the port's voice VLAN.

```
(config-if)# switchport voice vlan <vlan-id>
```

# Step 2

Set the port's trunk encapsulation protocol.

```
(config-if)# switchport trunk encapsulation dot1q
```

Manually configure trunk mode.

```
(config-if)# switchport mode trunk
```

Specify or modify the port's list of allowed VLANs (when in trunk mode).

```
(config-if)# switchport trunk allowed vlan {<vlans> | add <vlans> | remove <vlans> | except <vlans> | all | none}
```

Enable the interface.

```
(config-if)# no shutdown
```

Configure a subinterface (ROAS).

```
(config-if)# interface <interface.subif-number>
```

Specify the subinterface's VLAN ID.

```
(config-subif)# encapsulation dot1q <vlan> [native]
```

Set the subinterfaces's IP address/netmask.

```
(config-subif)# ip address <ip-address> <netmask>
```

# Step 3

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

# Step 4

## PH2's GUI

Call PH1's phone number.

- Dial 2010 > Pick up the phone
