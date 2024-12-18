## Creating VLAN:
```
Switch#configure terminal
Switch(config)#hostname DS1
DS1(config)#vlan 10
DS1(config-vlan)#name GREEN
DS1(config-vlan)#vlan 11
DS1(config-vlan)#name YELLOW
DS1(config-vlan)#vlan 12
DS1(config-vlan)#name BLUE
DS1(config-vlan)#vlan 13
DS1(config-vlan)#name RED
DS1(config-vlan)#vlan 999
DS1(config-vlan)#exit
```

## RSTP Configuration

```
DS1(config)#spanning-tree mode rapid-pvst
DS1(config)#spanning-tree vlan 10-13 priority 0
DS1(config)#interface range e0/1-2
DS1(config-if-range)#spanning-tree guard root
DS1(config-if-range)#
```

## Etherchannel Configuration

```
DS1(config)#interface range e0/1-2
DS1(config-if-range)#description DS1_TO_AS1
DS1(config-if-range)#shutdown
DS1(config-if-range)#channel-group 1 mode active
DS1(config-if-range)#switchport trunk encapsulation dot1q
DS1(config-if-range)#switchport mode trunk
DS1(config-if-range)#switchport nonegotiate
DS1(config-if-range)#switchport trunk allowed vlan 10-13
DS1(config-if-range)#switchport trunk native vlan 999
```

## Inter-VLAN Routing Configuration

```
DS1(config)#ip routing
DS1(config)#int vlan 10
DS1(config-if)#ip add 10.0.0.1 255.255.255.0
DS1(config-if)#int vlan 11
DS1(config-if)#ip add 10.0.1.1 255.255.255.0
DS1(config-if)#int vlan 12
DS1(config-if)#ip add 10.0.2.1 255.255.255.0
DS1(config-if)#int vlan 13
DS1(config-if)#ip add 10.0.3.1 255.255.255.0
DS1(config-if)#exit
DS1(config)#int e0/0
DS1(config-if)#description DS1_TO_CS
DS1(config-if)#no switchport
DS1(config-if)#ip add 10.0.255.14 255.255.255.252
```
## Root Guard

```
DS1(config)#interface po1
DS1(config-if)#spanning-tree guard root
```


