# Day 35 Lab - Extended ACLs

## Step 1

### PC1's Command Prompt

Specifies ping continue sending echo Request messages to the destination until interrupted.

```
ping pc2
```

Configure an extended named ACL

```
(config)#ip access-list extended <name>
```

Configure an ACE in the extended named ACL, matching based on protocol. src/dst IP, and src/dst port

```
(config-ext-nacl)#{permit | deny} {tcp | udp} <source> [<operator-src-port>] <destination> [<operator dst-port>]
```

Configure an ACE in the extended named ACL, matching based on protocol and source/destination IP

```
(config-ext-nacl)#{permit | deny} <protocol> <source> <destination>
```

Apply an ACL to an interface

```
(config-if)#ip access-group <acl> {in | out}
```

### PC1's Command Prompt

Specifies ping continue sending echo Request messages to the destination until interrupted.

```
ping srv2
```

```
ping 192.168.2.100
```

### PC3's Web Browser

Go to URL

```
cisco.com
```

### PC3's Command Prompt

Specifies ping continue sending echo Request messages to the destination until interrupted.

```
ping pc1
```

```
ping pc2
```

View all ACLs

```
#show access-lists
```
