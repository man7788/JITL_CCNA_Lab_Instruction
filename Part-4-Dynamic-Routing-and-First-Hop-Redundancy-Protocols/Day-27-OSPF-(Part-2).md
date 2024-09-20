# Day 27 Lab - OSPF (Part 2)

## Step 3

Activate OSPF on the interface

```
(config-if)#ip ospf <process-id> area <area>
```

View information about router's active routing protocols

```
#show ip protocols
```

Create/configure an OSPF process

```
(config)#router ospf <process-id>
```

Configure a passive interface

```
(config-router)#passive-interface <interface>
```

Make all interfaces passive by default

```
(config-router)#passive-interface default
```

Disable a passive interface

```
(config-router)#no passive-interface <interface>
```

View OSPF neighbors and their status

```
#show ip ospf neighbor
```

## Step 4

Modify the OSPF cost reference bandwidth

```
(config-router)#auto-cost reference-bandwidth <mbps>
```

View information about all OSPF interfaces

```
#show ip ospf interface
```

## Step 5

Advertise a default route to other routers

```
(config-router)#default-information originate
```

Configure a default route

```
(config)# ip route 0.0.0.0 0.0.0.0 <next-hop>
```

## Step 6

View the routing table

```
#show ip route
```

Disable the interface

```
(config-if)#shutdown
```
