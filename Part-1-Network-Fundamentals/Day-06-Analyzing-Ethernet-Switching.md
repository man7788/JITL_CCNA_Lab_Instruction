# Day 06 Lab - Analyzing Ethernet Switching

## Step 1

1. ARP Request (received by PC2, PC3, PC4)
2. ARP Reply (received by PC1)
3. ICMP Echo Request (received by PC3)
4. ICMP Echo Reply (received by PC1)

## Step 2

### PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

## Step 3

### PC2's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

## Step 4

View the switch's MAC address table.

```
# show mac address-table
```

## Step 5

Remove all dynamic MAC addresses.

```
# clear mac address-table dynamic
```
