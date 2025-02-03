# Day 17 Lab - VLANs (Part 2)

## Step 1

Manually configure access mode.

```
(config-if)# switchport mode access
```

Set the port's access VLAN.

```
(config-if)# switchport access vlan <vlan-id>
```

## Step 2

Manually configure trunk mode.

```
(config-if)# switchport mode trunk
```

Specify the port's list of allowed VLANs.

```
(config-if)# switchposrt trunk allowed vlan <vlans>
```

Specify the port's native VLAN.

```
(config-if)# switchposrt trunk native vlan <vlan-id>
```

View a list of VLANs and associated ports.

```
# show vlan brief
```

Configure a VLAN.

```
(config)# vlan <vlan-id>
```

## Step 3

### SW2

Manually configure trunk mode.

```
(config-if)# switchport mode trunk
```

Specify the port's list of allowed VLANs.

```
(config-if)# switchposrt trunk allowed vlan <vlans>
```

Specify the port's native VLAN.

```
(config-if)# switchposrt trunk native vlan <vlan-id>
```

### R1

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
(config-subif)# encapsulation dot1q <vlan>
```

Set the interfaces's IP address/netmask.

```
(config-subif)# ip address <ip-address> <netmask>
```

## Step 4

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```
