# Day 20 Lab - Analyzing STP

## Which switch is the root bridge?

SW3 - Lowest Bridge Priority

## Identify the role of each switch port

### SW1

- F0/1: Non-Designated
- F0/2: Non-Designated
- F0/3: Non-Designated
- F0/4: Root

### SW2

- F0/1: Designated
- F0/2: Designated
- F0/3: Non-Designated
- G0/1: Root

### SW3

- F0/1: Designated
- F0/2: Designated
- F0/3: Designated
- G0/1: Designated

### SW4

- G0/1: Designated
- G0/2: Root

## Confirm your answers in the CLI

View STP status and information

```
#show spanning-tree
```
