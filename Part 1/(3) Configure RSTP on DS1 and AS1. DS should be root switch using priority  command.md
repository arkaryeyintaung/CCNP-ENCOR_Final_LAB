# Configure RSTP on DS1 and AS1. DS should be root switch using priority command. 

## Configure RSTP
```
DS1>enable
DS1#configure terminal
DS1(config)#spanning-tree mode rapid-pvst
DS1(config)#spanning-tree vlan 10-13 priority 0
DS1(config)#interface range ethernet 0/1-2
DS1(config-if-range)#spanning-tree guard root
```
