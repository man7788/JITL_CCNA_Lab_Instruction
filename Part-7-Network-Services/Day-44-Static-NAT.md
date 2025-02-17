# Day 44 Lab - Static NAT

# Step 1

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

# Step 2

Configure an inside interface.

```
(config-if)# ip nat inside
```

Configure an outside interface.

```
(config-if)# ip nat outside
```

Configure a static NAT mapping.

```
(config)# ip nat inside source static <inside-local> <inside-global>
```

View the NAT translation table.

```
# show ip nat translations
```

View the NAT translation statistics.

```
# show ip nat statistics
```

# Step 3

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

# Step 4

### PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

##

View the NAT translation table.

```
# show ip nat translations
```

# Step 5

Clear the NAT translation table.

```
# clear ip nat translation *
```

View the NAT translation table.

```
# show ip nat translations
```
