# Day 04 Lab - Basic Device Security

## Step 1

### Enter privileged EXEC mode

```
>enable
```

### Enter global configuration mode

```
#configure terminal
```

### Set the device's hostname

```
(config)#hostname <hostname>
```

## Step 2

### Configure an unencrypted enable password

```
(config)#enable passoword <passowrd>
```

## Step 3

### Return to the previous level in the IOS CLI hierarchy

```
(config)#exit
```

## Step 4

### Show running-config

```
#show running-config
```

## Step 5

### Encrypt passwords in the configuration with type-7 encryption (weak)

```
(config)#service password-encryption
```

## Step 6

### Show running-config

```
#show running-config
```

## Step 7

### Configure a hashed enable secret

```
(config)#enable secret <password>
```

## Step 8

### Return to the previous level in the IOS CLI hierarchy

```
(config)#exit
```

## Step 9

### Show running-config

```
#show running-config
```

## Step 10

### Save the device configuration by copying the running-config to the startup-config

```
#write
```

```
#write memory
```

```
#copy running-config startup-config
```
