# Day 18 Lab - Multilayer Switching

## Step 1

### R1

Show running-config

```
#show running-config
```

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

Delete a subinterface (ROAS)

```
(config)#no interface <interface.subif-number>
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

### SW2

Show running-config

```
#show running-config
```

Set the interface to default configuration

```
(config)#default interface <interface>
```

Make the port a Layer 3 routed port

```
(config-if)#no switchport
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

View the routing table

```
#show ip route
```

Enable IP routing on a multilayer switch

```
(config)#ip routing
```

Configure a recursive static route

```
(config-if)#ip route <destination-network> <netmask> <next-hop>
```

## Step 2

View a list of VLANs and associated ports

```
#show vlan brief
```

Configure a switch virtual interface (SVI)

```
(config)#interface vlan <vlan-id>
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

## Step 3

### Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 10.0.0.xxx
```

## Step 4

### Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 1.1.1.1
```
