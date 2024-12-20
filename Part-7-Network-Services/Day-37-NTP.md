# Day 37 Lab - NTP

# Step 1

Set the time of the software clock

```
#clock set <hh:mm:ss> <month> <day> <year>
```

View the time of the software clock

```
#show clock [detail]
```

# Step 2

Set the device's time zone

```
(config)#clock timezone <name> <hours-offset> <minutes-offset>
```

View the time of the software clock

```
#show clock [detail]
```

# Step 3

Configure this device as an NTP client of the specified server

```
(config)#ntp server <ip-address> [prefer]
```

View a list of NTP associations (time sources)

```
#show ntp associations
```

View the device's NTP status

```
#show ntp status
```

View the time of the software clock

```
#show clock [detail]
```

# Step 4

Make this device a primary NTP server with its own clock as the referece clock

```
(config)#ntp master [stratum]
```

Configure an NTP authentication key

```
(config)#ntp authentication-key <key-number> md5 <key>
```

Specify an NTP trusted authentication key

```
(config)#ntp trusted-key <key-number>
```

Configure this device as an NTP client of the specified server and authenticate it with the specified key

```
(config)#ntp server <ip-address> key <key-number>
```

View a list of NTP associations (time sources)

```
#show ntp associations
```

View the time of the software clock

```
#show clock [detail]
```

# Step 5

Use NTP to regularly update the calendar

```
(config)#ntp update-calendar
```

View the time of the hardware calendar

```
#show calendar
```
