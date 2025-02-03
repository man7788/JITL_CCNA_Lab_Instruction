# Day 09 Lab - Configuring Interfaces

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

Set the interfaces's IP address/netmask.

```
(config-if)# ip address <ip-address> <netmask>
```

##
### PC's Config GUI > INTERFACE > FastEthernet0

#### IP Configuration > Static

- Configure IP Address.

- Configure Subnet Mask.


## Step 3

View interface status, speed, and duplex.

```
# show interfaces status
```

Set the interfaces's speed.

```
(config-if)# speed {auto | <speed>}
```

Set the interfaces's duplex.

```
(config-if)# speed {auto | full | half}
```

## Step 4

Set the interfaces's description.

```
(config-if)# description <description>
```

Enable/disable the interface.

```
(config-if)# [no] shutdown
```



## Step 5

Enable/disable the interface.

```
(config-if)# [no] shutdown
```

## Step 6

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

View the startup-config.

```
# show startup-config
```