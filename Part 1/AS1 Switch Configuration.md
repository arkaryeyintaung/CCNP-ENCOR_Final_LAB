







```

AS1(config)#int e0/2
AS1(config-if)#switchport mode access
AS1(config-if)#switchport access vlan 10
AS1(config-if)#spanning-tree portfast
AS1(config-if)#switchport port-security mac-address sticky
AS1(config-if)#switchport port-security maximum 1
AS1(config-if)#end
```
