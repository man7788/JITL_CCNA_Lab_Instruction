# Day 21 Lab - Configuring Spanning Tree

## Step 1

View STP status and information

```
#show spanning-tree
```

## Step 2

Set the bridge priority to 24576, or the lowest increment of 4096 needed to become the root bridge

```
(config)#spanning-tree vlan <vlan> root primary
```

Set the bridge priority to 28672

```
(config)#spanning-tree vlan <vlan> root secondary
```

View STP status and information

```
#show spanning-tree
```

## Step 3

View VLAN STP status and information

```
#show spanning-tree <vlan>
```

Configures the spanning tree cost for the VLAN

```
(config-if)#spanning-tree vlan <vlan> cost <cost>
```

## Step 4

View VLAN STP status and information

```
#show spanning-tree <vlan>
```

Configures the spanning tree cost for the VLAN

```
(config-if)#spanning-tree vlan <vlan> cost <cost>
```

## Step 5

1.  Turn on link lights for this step

    - Options > Preferences > Show Link Lights

2.  Delete connection between SW3 and PC1
3.  Connect SW3 to PC1 again, it should take about 30 seconds to re-connect

4.  Enable Portfast on the port

    ```
    (config-if)#spanning-tree portfast
    ```

    Enable BPDU Guard on the port

    ```
    (config-if)#spanning-tree bpduguard enable
    ```

5.  Delete connection between SW3 and PC1
6.  Connect SW3 to PC1 again, it should re-connect immediately
7.  Delete connection between SW3 and PC1
8.  Connect SW3 to SW4, SW3 should shut down
9.  Delete connection between SW3 and SE4
10. Connect SW3 to PC1 again
11. Enable/disable the interface

    ```
    (config-if)#[no] shutdown
    ```

12. SW3 and PC1 should re-connect
