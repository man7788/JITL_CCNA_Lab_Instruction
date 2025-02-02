# Day 08 Lab - Configuring IP Addresses

## Step 1

Set the device's hostname.

```
(config)# hostname <hostname>
```

## Step 2

View a concise summary of interface IP addresses and status.

```
# show ip interface brief
```

## Step 3

Enter interface config mode for the specified interface.

```
(config)# interface <interface>
```

Set the interfaces's IP address/netmask.

```
(config-if)# ip address <ip-address> <netmask>
```

Set the interfaces's description.

```
(config-if)# description <description>
```

Enable/disable the interface.

```
(config-if)# [no] shutdown
```

## Step 4

Return to privileged EXEC mode from any configuration mode.

```
(config-if)# end
```

View a concise summary of interface IP addresses and status.

```
# show ip interface brief
```

## Step 5

View the running-config.

```
# show running-config
```

Save the device configuration by copying the running-config to the startup-config.

```
# write
```

```
# write memory
```

```
# copy running-config startup-config
```

## Step 6

### PC's Config GUI > INTERFACE > FastEthernet0

#### IP Configuration > Static

- Configure IP Address.

- Configure Subnet Mask.


## Step 7

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```
