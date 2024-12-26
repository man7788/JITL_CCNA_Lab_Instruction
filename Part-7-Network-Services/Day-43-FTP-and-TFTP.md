# Day 43 Lab - FTP-and-TFTP

# Step 1

## SRV1

1. Config Default Gateway
2. Config Interface's IP Address
3. Config Interface's Subnet Mask

##

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

Enable/disable the interface

```
(config-if)#[no] shutdown
```

Configure a recursive static route

```
(config-if)#ip route <destination-network> <netmask> <next-hop>
```

# Step 2

View information about the IOS version

```
#show version
```

View the contents of flash memory

```
show flash:
```

Copy a file from TFTP server to flash

```
copy tftp: flash:
```

# Step 3

Set the IOS image that will be loaded on the next boot

```
(config)#boot system <image-path>
```

Save the device configuration by copying the running-config to the startup-config

```
#write
```

Reload the operating system

```
#reload
```

View information about the IOS version

```
#show version
```

View the contents of flash memory

```
#show flash:
```

Delete a file from Flash with a specified file name

```
#delete flash:<file-name>
```

# Step 4

View information about the IOS version

```
#show version
```

Set the default FTP username

```
(config)#ip ftp username <username>
```

Set the default FTP password

```
(config)#ip ftp username <password>
```

Copy a file from FTP server to flash

```
copy ftp: flash:
```

View the contents of flash memory

```
show flash:
```

# Step 5

Set the IOS image that will be loaded on the next boot

```
(config)#boot system <image-path>
```

Save the device configuration by copying the running-config to the startup-config

```
#write
```

Reload the operating system

```
#reload
```

View information about the IOS version

```
#show version
```

View the contents of flash memory

```
#show flash:
```

Delete a file from Flash with a specified file name

```
#delete flash:<file-name>
```
