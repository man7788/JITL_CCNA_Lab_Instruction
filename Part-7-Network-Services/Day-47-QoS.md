# Day 47 Lab - QoS

# Step 1 - 3

Create a class map for matching packets to a specified class.

```
# class-map { [type inspect match-all] | [ match-any ] } <class-map-name>
```

Configure a match condition based on layer 7 protocol for the class map.

```
(config-cmap)# match protocol <protocol>
```

View the running-config, section class-map.

```
# show running-config | section class-map
```

Configure a policy map.

```
# policy-map <policymap-name>
```

Configure the service policy for a class map.

```
(config-pmap)# class <class-map-name>
```

Configure the DSCP marking in a optimization policy.

```
(config-pmap-c)# set ip dscp <dscp-marking>
```

Assigns priority to a traffic class at the priority level specified.

```
(config-pmap-c)# priority percent <percentage-value>
```

Specify the minimum bandwidth allocated to a class belonging to a policy map.

```
(config-pmap-c)# bandwidth { rate [units] | percent <percentage-value> }
```

Attach a policy map to an input interface.

```
(config-if)# service-policy [type access-control] {input | output} <policy-map-name>
```

View the running-config, section policy-map.

```
# show running-config | section policy-map
```

View the running-config.

```
# show running-config
```

# Step 4

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

### PC's Desktop > Web Browser

- Go to specific HTTP/HTTPS URLs in web browser.

##

Conversion from DSCP hexidecimal to AF marking system:
1. Convert the two hexidecimal nubmers to two groups of four binary numbers (e.g. 1A = 0001 1010).

2. Combine the two binary number groups into one binary group (e.g. 00011010).

3. Take only six least significant binary numbers and map them to DSHP IP header field (e.g. 011010 = AF31).