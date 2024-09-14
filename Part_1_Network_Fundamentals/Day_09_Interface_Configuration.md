# Day 09 Lab - Interface Configuration

## Step 1

Set the device's hostname

```
(config)#hostname <hostname>
```

## Step 2

### Router

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

### PC

1. Config all PC's Interface IP Address
2. Config all PC's Interface Subnet Mask

## Step 3

### Router

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

### Switch

View interface status, speed, and duplex

```
#show interfaces status
```

### Configuration

Set the interfaces's speed

```
(config-if)#speed {auto | <speed>}
```

Set the interfaces's duplex

```
(config-if)#speed {auto | full | half}
```

## Step 4

Set the interfaces's description

```
(config-if)#description <description>
```

Enable/disable the interface

```
(config-if)#[no] shutdown
```

Show running-config

```
#show running-config
```

Save the device configuration by copying the running-config to the startup-config

```
#write
```

```
#write memory
```

```
#copy running-config startup-config
```
