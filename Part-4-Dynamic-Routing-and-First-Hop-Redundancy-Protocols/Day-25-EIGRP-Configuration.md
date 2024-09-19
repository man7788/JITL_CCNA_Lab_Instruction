# Day 25 Lab - EIGRP Configuration

## Step 2

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

Create/configure a loopback interface

```
interface loopback <number>
```

Set the interfaces's IP address/netmask

```
(config-if)#ip address <ip-address> <netmask>
```

## Step 3

Create/configure an EIGRP process

```
(config)#router eigrp <as-number>
```

Activate EIGRP on all interfaces

```
(config-router)#network 0.0.0.0 255.255.255.255
```

> Not recommended on real networks

View information about router's active routing protocols

```
#show ip protocols
```

Disable automatic network summarization

```
(config-router)#no auto-summary
```

Configure a passive interface

```
(config-router)#passive-interface <interface>
```

Activate EIGRP on interfaces with an IP address in the specified range

```
(config-router)#network <ip-address> <wildcard-mask>
```

View EIGRP neighbors and their status

```
#show ip eigrp neighbor
```

View the routing table

```
#show ip route [protocol]
```

To display Enhanced Interior Gateway Routing Protocol (EIGRP) topology table entries

```
#show ip eigrp topology
```

## Step 4

View information about router's active routing protocols

```
#show ip protocols
```

Instructs the router to include routes with a metric less than or equal to n times the minimum metric route for that destination, where n is the number specified by the variance command

```
(config-router)#variance <n>
```
