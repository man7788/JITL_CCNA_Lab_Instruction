# Day 19 Lab - DTP & VTP

## Step 1

Show interface switchport information

```
#show interfaces <interface-id> switchport
```

Manually configure trunk mode

```
(config-if)#switchport mode trunk
```

Disable DTP on the port

```
(config-if)#switchport nonegotiate
```

## Step 2

View VTP information

```
#show vtp status
```

Set the VTP domain name

```
(config)#vtp domain <name>
```

Configure a VLAN

```
(config)#vlan <vlan-id>
```

View a list of VLANs and associated ports

```
#show vlan brief
```

## Step 3

Set the VTP mode

```
(config)#vtp mode transparent
```

Configure a VLAN

```
(config)#vlan <vlan-id>
```

View VTP information

```
#show vtp status
```

## Step 4

Set the VTP mode

```
(config)#vtp mode client
```

Configure a VLAN

```
(config)#vlan <vlan-id>
```

## Step 5

Show interface switchport information

```
#show interfaces <interface-id> switchport
```

Set the VTP mode

```
(config)#vtp mode access
```

Set the port's access VLAN

```
(config-if)#switchport access vlan <vlan-id>
```
