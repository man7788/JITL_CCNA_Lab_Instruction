# Day 44 Lab - NAT Part 1

# Step 1

## PC1

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 8.8.8.8
```

##

# Step 2

Configure an inside interface

```
(config-if)#ip nat inside
```

Configure an outside interface

```
(config-if)#ip nat outside
```

Configure a static NAT mapping

```
(config)#ip nat inside source static <inside-local> <inside-global>
```

View the NAT translation table

```
#show ip nat translations
```

View the NAT translation statistics

```
#show ip nat statistics
```

# Step 3

## PC1

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping 8.8.8.8
```

# Step 4

## PCs

Send Internet Control Message Protocol (ICMP) echo Request messages

```
ping google.com
```

##

View the NAT translation table

```
#show ip nat translations
```

# Step 5

Clear the NAT translation table

```
#clear ip nat translation *
```

View the NAT translation table

```
#show ip nat translations
```
