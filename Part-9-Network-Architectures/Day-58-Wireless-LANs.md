# Day 58 Lab - Wireless LANs

View the running-config.

```
# show running-config
```

# Step 1

### PC's Desktop > Web Browser

#### Access GUI of WLC1
- URL: https://172.16.1.10


# Step 2

### WLC1's GUI

View AP Join Statistics

- Monitor > Statistics > AP Join

# Step 3

## WLC1's GUI

### Create a dynamic interface for Internal WLAN

1. Interfaces > New

- Interface Name: Internal
- VLAN Id: 100

2. Interfaces > Edit

- Physical Information

  - Port Number: 1

- Interface Address

  - VLAN Indentifier: 100
  - IP Address: 10.0.0.10
  - Netmask: 255.255.255.0
  - Gateway: 10.0.0.1

- DHCP Information

  - Primary DHCP Server: 10.0.0.1

### Create a dynamic interface for Guest WLAN

1. Interfaces > New

- Interface Name: Guest
- VLAN Id: 200

2. Interfaces > Edit

- Physical Information

  - Port Number: 1

- Interface Address

  - VLAN Indentifier: 200
  - IP Address: 10.1.0.10
  - Netmask: 255.255.255.0
  - Gateway: 10.1.0.1

- DHCP Information

  - Primary DHCP Server: 10.1.0.1


# Step 4

## WLC1's GUI

### Create the Internal WLAN using WPA-2 + PSK

1. WLANs > New

- Profile Name: Internal
- SSID: Internal
- ID: 1

2. WLANs > Edit 'Internal' > General

- Status: ✔ Enabled
- Interface/Interface Group(G): Internal

3. WLANs > Edit 'Internal' > Security > Layer 2

- Layer 2 Security: WPA + WPA2

- WPA + WPA2 Parameters

  - WPA2 Policy: ✔
  - WPA2 Encryption: ✔ AES

- Authentication Key Management

  - PSK: ✔ Enabled
  - PSK Format: ASCII
    - Cisco123

### Create the Guest WLAN using WPA-2 + PSK

1. WLANs > New

- Profile Name: Guest
- SSID: Guest
- ID: 2

2. WLANs > Edit 'Guest' > General

- Status: ✔ Enabled
- Interface/Interface Group(G): Guest

3. WLANs > Edit 'Internal' > Security > Layer 2

- Layer 2 Security: WPA + WPA2

- WPA + WPA2 Parameters

  - WPA2 Policy: ✔
  - WPA2 Encryption: ✔ AES

- Authentication Key Management

  - PSK: ✔ Enabled
  - PSK Format: ASCII
    - Cisco123


# Step 5

Add a smartphone to the network

- End Devices > Smart Phone

## Smartphone0

Join the Internal SSID

- Config > INTERFACE > Wireless0

  - SSID: Internal
  - Authentication
    - WPA2-PSK
      - PSK Pass Phrase: Cisco123
