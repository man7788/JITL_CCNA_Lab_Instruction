# Day 22 Lab - Rapid STP

## Step 1

View STP status and information.

```
# show spanning-tree
```

Which switch is the root bridge?

- SW1 - Lowest MAC Address

What appears different than what you have learned about the root bridge?

- There is a backup port in the root bridge.

What is the cause of this?

- All ports of a root bridge are designated ports, and there is only one designated port per collision domain.

## Step 2

### SW1

- F0/1: Designated
- F0/2: Designated
- F0/3: Backup

### SW2

- F0/1: Root
- F0/2: Designated
- G0/1: Alternate

### SW3

- F0/1: Designated
- F0/2: Root
- G0/1: Designated

### SW4

- F0/1: Root
- F0/2: Alternate
- F0/24: Designated

> All ports connecting to the end hosts are all designated ports.

View STP status and information.

```
# show spanning-tree
```

## Step 3

View STP status and information.

```
# show spanning-tree
```

Set the port's RSTP link type.

```
(config-if)# spanning-tree link-type {point-to-point | shared}
```



Enable Portfast on the port.

```
(config-if)# spanning-tree portfast
```

> Edge ports connecting to the end hosts are also point-to-point links, if they are operating at full-duplex mode.

> Edge ports connecting to a hub are also shared links, the hub doesn't exist in terms of spanning-tree.
