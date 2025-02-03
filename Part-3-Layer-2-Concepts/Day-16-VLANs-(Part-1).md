# Day 16 Lab - VLANs (Part 1)

## Step 1

### PC's Config GUI > GLOBAL > Settings

#### Gateway/DNS IPv4 > Static

- Configure Default Gateway.

### PC's Config GUI > INTERFACE > FastEthernet0

#### IP Configuration > Static

- Configure IP Address.

- Configure Subnet Mask.


## Step 2

Make 3 Copper Straight-Through cable connections.

- SW1 -> R1

Set the interfaces's IP address/netmask.

```
(config-if)# ip address <ip-address> <netmask>
```

Enable the interface.

```
(config-if)# no shutdown
```

View a concise summary of interface IP addresses and status.

```
# show ip interface brief
```

## Step 3

Manually configure access mode.

```
(config-if)# switchport mode access
```

Set the port's access VLAN.

```
(config-if)# switchport access vlan <vlan-id>
```

View a list of VLANs and associated ports.

```
# show vlan brief
```

Configure a VLAN.

```
(config)# vlan <vlan-id>
```

Name the VLAN.

```
(config-vlan)# name <name>
```

## Step 4


### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```
