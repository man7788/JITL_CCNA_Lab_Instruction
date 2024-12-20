# Day 36 Lab - CDP and LLDP

# Step 1

Display all current TCP/IP network configuration values

## PC

```
ipconfig
```

##

View information about CDP neighbors

```
#show cdp neighbors [detail]
```

View interface status, speed, and duplex

```
#show interfaces status
```

View interface Layer 1/2 information

```
#show interfaces [interface]
```

View detailed information about the specified CDP neighbor

```
#show cdp entry <name>
```

# Step 2

View information about CDP interfaces

```
#show cdp interface [interface]
```

Enable/disable CDP on an interface

```
(config-if)#[no] cdp enable
```

# Step 3

Globally enable/disable CDP

```
(config)#[no] cdp run
```

# Step 4

Globally enable/disable LLDP

```
(config)#[no] lldp run
```

Enable/disable LLDP Tx on the interface

```
(config-if)#[no] lldp transmit
```

Enable/disable LLDP Rx on the interface

```
(config-if)#[no] lldp receive
```
