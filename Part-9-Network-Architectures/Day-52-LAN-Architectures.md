# Day 52 Lab - LAN Architectures

View HSRP status and information

```
#show standby [brief]
```

View VLAN STP status and information

```
#show spanning-tree <vlan>
```

Set the bridge priority to 24576, or the lowest increment of 4096 needed to become the root bridge

```
(config)#spanning-tree vlan <vlan> root primary
```

Set the bridge priority to 28672

```
(config)#spanning-tree vlan <vlan> root secondary
```

Configure a switch virtual interface (SVI)

```
(config)#interface vlan <vlan-id>
```

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
