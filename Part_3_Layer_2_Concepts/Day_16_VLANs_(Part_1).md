# Day 16 Lab - VLANs (Part 1)

## Step 1

### PC

1. Config all PC's Default Gateway
2. Config all PC's Interface IP Address
3. Config all PC's Interface Subnet Mask

## Step 2

### Copper Straight-Through

1. SW1 -> R1

### Router

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

Enablethe interface

```
(config-if)#no shutdown
```

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

## Step 3

Manually configure access mode

```
(config-if)#switchport mode access
```

Set the port's access VLAN

```
(config-if)#switchport access vlan <vlan-id>
```

View a list of VLANs and associated ports

```
#show vlan brief
```

Configure a VLAN

```
(config)#vlan <vlan-id>
```

Name the VLAN

```
(config-vlan)#name <name>
```

## Step 4

### Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 10.0.0.xxx
```
