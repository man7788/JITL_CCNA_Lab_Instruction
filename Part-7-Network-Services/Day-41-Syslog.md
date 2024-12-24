# Day 41 Lab - Syslog

# Step 1

Enable/disable the interface

```
(config-if)#[no] shutdown
```

View a concise summary of interface IP addresses and status

```
#show ip interface brief
```

Timestamp log messages with the current date and time

```
(config-if)#service timestamps log datetime [locatime] [msec]
```

# Step 2

## PC

Communicates with a computer running the telnet server service

```
telnet 192.168.1.1
```

##

Enable/disable the interface

```
(config-if)#[no] shutdown
```

Enable real-time logging to the VTY lines for the current session

```
#terminal monitor
```

# Step 3

Show Syslog settings and the logging buffer

```
#show logging
```

Configure logging to the logging buffer

```
(config-if)#logging buffered [<bytes>] [<severity>]
```

# Step 4

Specify the Syslog server to send logs to

```
(config-if)#logging [host] <ip-address>
```

Configure logging to a Syslog server

```
(config-if)#logging trap [<severity>]
```

## Server 1

View Syslog server logging

- SRV1 > Services > SYSLOG

##
