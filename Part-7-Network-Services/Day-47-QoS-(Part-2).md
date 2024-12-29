# Day 47 Lab - QoS Part 2

# Step 1 - 3

Create a class map for matching packets to a specified class

```
#class-map { [type inspect match-all] | [ match-any ] } <class-map-name>
```

Configure a match condition based on layer 7 protocol for the class map

```
(config-cmap)#match protocol <protocol>
```

View the running-config, section class-map

```
#show running-config | section class-map
```

Configure a policy map

```
#policy-map <policymap-name>
```

Configure the service policy for a class map

```
(config-pmap)#class <class-map-name>
```

Configure the DSCP marking in a optimization policy

```
(config-pmap-c)#set ip dscp <dscp-marking>
```

Assigns priority to a traffic class at the priority level specified

```
(config-pmap-c)#priority percent <percentage-value>
```

Specify the minimum bandwidth allocated to a class belonging to a policy map

```
(config-pmap-c)#bandwidth { rate [units] | percent <percentage-value> }
```

Attach a policy map to an input interface

```
(config-if)#service-policy [type access-control] {input | output} <policy-map-name>
```

View the running-config, section policy-map

```
#show running-config | section policy-map
```

Show running-config

```
#show running-config
```

# Step 4

## PC1

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 10.0.0.100
```

Go to a specified URL in web browser

```
http://10.0.0.100
```

```
https://10.0.0.100
```
