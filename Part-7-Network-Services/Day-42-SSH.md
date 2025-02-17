# Day 42 Lab - SSH

# Step 1

Connect Laptop1's RS232 port to SW2's console port.

- Connections > Console

### PC's Desktop > Terminal

Set the device's hostname.

```
(config)# hostname <hostname>
```

Configure a hashed enable secret.

```
(config)# enable secret <password>
```

Create a local user account.

```
(config)# username <username> secret <password>
```

Configure a switch virtual interface (SVI).

```
(config)# interface vlan <vlan-id>
```

Set the interfaces's IP address/netmask.

```
(config-if)# ip address <ip-address> <netmask>
```

Enable/disable the interface.

```
(config-if)# [no] shutdown
```

Set the Layer 2 switch's default gateway.

```
(config)# ip default-gateway <ip-address>
```

# Step 2

Configure the console line.

```
(config)# line console 0
```

Require a user to log in with a local user accounut to access the line.

```
(config-line)# login local
```

Set the inactivity logout timer.

```
(config-line)# exec-timeout <minutes>
```

# Step 3

Set the devices's default domain name.

```
(config)# ip domain name <domain-name>
```

Generate an RSA key pair (for SSH).

```
(config)# crypto key generate rsa
```

Configure an ACE in a standard numbered ACL for a single host address.

```
(config)# access-list <number> {permit|deny} host <ip-address>
```

Configure all 16 VTY lines.

```
(config)# line vty 0 15
```

Require a user to log in with a local user account to access the line.

```
(config-line)# login local
```

Set the inactivity logout timer.

```
(config-line)# exec-timeout <minutes>
```

Set the protocols that can be used to connect to the line.

```
(config-line)# transport input {telnet | ssh | all | none}
```

Apply an ACL to limit access to the line.

```
(config-line)# access-class <acl> in
```

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
# ping <targetname>
```

Connect to a device using a username and password.

```
# ssh -l <username> <ip-address>
```

or

```
# ssh <username>@<ip-address>
```
## PC1's Command Prompt

Send Internet Control Message Protocol (ICMP) echo Request messages.

```
> ping 192.168.2.253
```

Connect to a device using a username and password.

```
> ssh -l <username> <ip-address>
```

or

```
> ssh <username>@<ip-address>
```
