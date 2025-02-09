# Day 29 Lab - HSRP Configuration

## Step 1

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

Display all current TCP/IP network configuration values.

```
> ipconfig
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
> tracert <targetname>
```

## Step 2

Enable HSRP version 2.

```
(config-if)# standby version 2
```

Set the HSRP virtual IP address.

```
(config-if)# standby <group> ip <virtual-ip>
```

Set the HSRP virtual IP priority.

```
(config-if)# standby <group> priority <priority>
```

Enable HSRP preemption.

```
(config-if)# standby <group> preempt
```

View HSRP status and information.

```
# show standby
```

## Step 3

### PC's Config GUI > GLOBAL > Settings

#### Gateway/DNS IPv4 > Static

- Configure Default Gateway.

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

Displays current arp cache tables for all interfaces.

```
> arp -a
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
> tracert <targetname>
```

## Step 4

Save the device configuration by copying the running-config to the startup-config.

```
# write
```

### PC's Physical GUI > Physical Device View

- Turn OFF the Power Switch.

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
> tracert <targetname>
```

## Step 5

### PC's Physical GUI > Physical Device View

- Turn ON the Power switch.

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

Trace the path that an Internet Protocol (IP) packet takes to its destination.

```
> tracert <targetname>
```
