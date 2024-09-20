# Day 29 Lab - HSRP Configuration

## Step 1

### PC Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 8.8.8.8
```

Display all current TCP/IP network configuration values

```
ipconfig
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
tracert 8.8.8.8
```

## Step 2

Enable HSRP version 2

```
(config-if)#standby version 2
```

Set the HSRP virtual IP address

```
(config-if)#standby <group> ip <virtual-ip>
```

Set the HSRP virtual IP priority

```
(config-if)#standby <group> priority <priority>
```

Enable HSRP preemption

```
(config-if)#standby <group> preempt
```

View HSRP status and information

```
#show standby
```

## Step 3

### PC

1. Config all PC's Default Gateway

### PC Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 8.8.8.8
```

Displays current arp cache tables for all interfaces

```
arp -a
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
tracert 8.8.8.8
```

## Step 4

Save the device configuration by copying the running-config to the startup-config

```
#write
```

Turn off a router

- Physical tab > Power switch

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 8.8.8.8
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
tracert 8.8.8.8
```

## Step 5

Save the device configuration by copying the running-config to the startup-config

```
#write
```

Turn on a router

- Physical tab > Power switch

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 8.8.8.8
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
tracert 8.8.8.8
```
