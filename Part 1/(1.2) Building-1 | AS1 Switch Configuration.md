
```
AS1#configure terminal
AS1(config)#hostname DS1
AS1(config)#vlan 10
AS1(config-vlan)#name GREEN
AS1(config-vlan)#vlan 11
AS1(config-vlan)#name YELLOW
AS1(config-vlan)#vlan 12
AS1(config-vlan)#name BLUE
AS1(config-vlan)#vlan 13
AS1(config-vlan)#name RED
AS1(config-vlan)#vlan 999
exit
```
----

```
AS1(config)#spanning-tree mode rapid-pvst
```
----

```
interface range e0/0-1
shut
channel-group 1 mode passive
switchport trunk encapsulation dot1q
switchport mode trunk
switchport nonegotiate
switchport trunk allow vlan 10-13
switchport trunk native vlan 999
```

---

```

AS1(config)#int e0/2
AS1(config-if)#switchport mode access
AS1(config-if)#switchport access vlan 10
AS1(config-if)#spanning-tree portfast
AS1(config-if)#switchport port-security mac-address sticky
AS1(config-if)#switchport port-security maximum 1
AS1(config-if)#end
```
