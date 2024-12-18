
```
DS1(config)#interface range ethernet 0/1-2
DS1(config-if-range)#Description DS1_TO_AS1
DS1(config-if-range)#shut
DS1(config-if-range)#channel-group 1 mode active
DS1(config-if-range)#switchport trunk encapsulation dot1q
DS1(config-if-range)#switchport mode trunk
DS1(config-if-range)#switchport nonegotiate
DS1(config-if-range)#switchport trunk allowed vlan 10-13
DS1(config-if-range)#switchport trunk native vlan 999
```
