# Create VLANs on site1 switches according to diagram.  

## Creating VLAN:
```
AS1(config)#vlan 10
AS1(config-vlan)#name GREEN
AS1(config-vlan)#vlan 11
AS1(config-vlan)#name YELLOW
AS1(config-vlan)#vlan 12
AS1(config-vlan)#name BLUE
AS1(config-vlan)#vlan 13
AS1(config-vlan)#name RED
```

---

## Assigning VLAN to an Interface:
```
AS1(config)#interface e0/2
AS1(config-if)#switchport mode access
AS1(config-if)#switchport access vlan 10
AS1(config-if)#exit
AS1(config)#interface e0/3
AS1(config-if)#switchport mode access
AS1(config-if)#switchport access vlan 11
AS1(config-if)#exit
AS1(config)#interface e1/0
AS1(config-if)#switchport mode access
AS1(config-if)#switchport access vlan 12
AS1(config-if)#exit
AS1(config)#interface e1/1
AS1(config-if)#switchport mode access
AS1(config-if)#switchport access vlan 13
AS1(config-if)#exit
```

## To check the VLAN configuration:
```
AS1(config)#do show vlan brief
```
![image](https://github.com/user-attachments/assets/21eb9b2c-6a59-4738-b742-9d2de13257bf)
