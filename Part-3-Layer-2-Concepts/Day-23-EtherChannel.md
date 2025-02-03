# Day 23 Lab - EtherChannel

## Step 1

View STP status and information.

```
# show spanning-tree
```

Configure an LACP EtherChannel.

```
(config-if)# channel-group <group> mode {active | passive}
```

Configure the port-channel interface.

```
(config)# interface port-channel <number>
```

Manually configure trunk mode.

```
(config-if)# switchport mode trunk
```

View the running-config.

```
# show running-config
```

View EtherChannel status.

```
# show ehterchannel summary
```

Set the port's trunk encapsulation protocol.

```
(config-if)# switchport trunk encapsulation dot1q
```

View a list of trunk ports.

```
# show interfaces trunk
```

## Step 2

Configure a PaGP EtherChannel.

```
(config-if)# channel-group <group> mode {desirable | auto}
```

Configure the port-channel interface.

```
(config)# interface port-channel <number>
```

Manually configure trunk mode.

```
(config-if)# switchport mode trunk
```

Set the port's trunk encapsulation protocol.

```
(config-if)# switchport trunk encapsulation dot1q
```

View EtherChannel status.

```
# show ehterchannel summary
```

## Step 3

Make the port a Layer 3 routed port.

```
(config-if)# no switchport
```

Configure a static EtherChannel.

```
(config-if)# channel-group <group> mode on
```

Configure the port-channel interface.

```
(config)# interface port-channel <number>
```

Set the interfaces's IP address/netmask.

```
(config-if)# ip address <ip-address> <netmask>
```

View EtherChannel status.

```
# show ehterchannel summary
```

To determine the network connectivity to another network device.

```
# ping <dest-address>
```

## Step 4

View the routing table.

```
# show ip route
```

Enable IP routing on a multilayer switch.

```
(config)# ip routing
```

Configure a recursive static route.

```
(config)# ip route <destination-network> <netmask> <next-hop>
```

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

## Step 5

View the load-balancing parameters.

```
# show etherchannel load-balance
```

## Step 6

Modify the EtherChannel load-balancing parameters.

```
(config)# port-channel load-balance <parameters>
```
