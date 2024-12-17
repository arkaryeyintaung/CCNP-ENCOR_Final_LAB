<h1 align="center">Task 1 Building 1</h1> 

- Create VLANs on site1 switches according to diagram.  
- Configure RSTP on DS1 and AS1. DS should be root switch using priority command. 
- Configure Layer 2 EtherChannel between DS1 and AS1 using industry standard protocol for negotiation. 
- Only DS1 should actively negotiate the EtherChannel negotiation. 
- Configure inter-vlan routing on DS1 so that all vlan can communicate to each other. 
- Configure all inter-switch links on DS1 and AS1 to be in static trunk.  
- Ensure that DTP is disable.  
- Configure the trunk encapsulation on DS1’s inter-switch links as 802.1q. 
- Configure the switches so that traffic between devices in VLAN 999 is not tagged when sent over the trunk links. 
- Configure ports Ethernet0/2 to E1/1 on AS1 to be access ports in respective VLAN. 
- Configure Spanning-Tree Port Fast on access ports so that access port does not have to wait for the Spanning-Tree listening and learning phases to begin forwarding and enable port security on access ports. 
- Configure DS1 so that STP logically blocks Ethernet links connected to AS1 if AS1 tries to become Root Bridge for any VLAN. 
- Configure DS1 to limit unicast traffic received from AS1 to 100Mbps. 
- Configure DS to limit broadcast traffic received from AS1 to 10Mbps.

![image](https://github.com/user-attachments/assets/0d46788a-1344-4c92-8ae0-fe7e8835c7a1)

---
