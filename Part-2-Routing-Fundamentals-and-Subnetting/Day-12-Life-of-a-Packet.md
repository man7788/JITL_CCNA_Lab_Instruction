# Day 12 Lab - Life of a Packet

## PC's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping <targetname>
```

Displays the full TCP/IP configuration for all adapters.

```
> ipconfig /all
```

## Router

View interface Layer 1/2 information.

```
# show interfaces [interface]
```

View the running-config.

```
# show running-config
```

## Step 1

### A

- 1111 >> AAAA

### B

- 1111 >> AAAA

### C

- BBBB >> CCCC

### D

- DDDD >> EEEE

### E

- FFFF >> 4444

### F

- FFFF >> 4444

## Step 2

### A

- 1111 >> 3333

### B

- 1111 >> 3333

## Step 3

### PC4 to R3 

- 4444 >> FFFF

### R3 to R2 

- EEEE >> DDDD

### R2 to R1 

- CCCC >> BBBB

### R1 to PC1 

- AAAA >> 1111
