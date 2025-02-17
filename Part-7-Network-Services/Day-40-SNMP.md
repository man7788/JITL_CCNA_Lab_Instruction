# Day 40 Lab - SNMP

# Step 1

Configure a read-only community string.

```
(config)# snmp-server community <password> ro
```

Configure a read-write community string.

```
(config)# snmp-server community <password> rw
```

# Step 2

### PC's Desktop > MIB Browser

- Address: 192.168.1.254
- Advanced...
  - Enter Read Community
  - Enter Write Community
- SNMP MIBS > router_std MIBs > .iso > .org > .dod > .internet > .mgmt > .mib-2
  - (Complete the rest of the lab in this directory)

1. #### How long has R1 been running? (system uptime)

- .system > .sysUpTime

- Operations: Get

2.  #### What is the currently configured hostname on R1?

- .system > .sysName

- Operations: Get

3. #### How many interfaces does R1 have?

- .interfaces > .ifNumber

- Operations: Get

4. #### What are those interfaces?

- .interfaces > .ifTable > .ifEntry > .ifDescr

- Operations: Get

- .interfaces > .ifTable > .ifEntry > .ifType

- Operations: Get

##

# Step 3

### PC's Desktop > MIB Browser

- .system > .sysName

- Operations: Get

- Operations: Set
  - Date Type: OctetString
  - Enter Value

##

View the running-config, limit output to hostname.

```
# show running-config | include hostname
```
