![image](https://github.com/user-attachments/assets/c7b51903-b9af-48e8-8bee-9b8c89ea1f4b)

<h1 align="center">CCNP-ENCOR_Final_LAB</h1> 

---

<h2 align="center">Part 1 Site 1 Building 1</h2> 

![image](https://github.com/user-attachments/assets/7d2f70fc-217e-41b4-8c08-00a8d03ceba7)

Task 1 Building 1
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
- Configure DS1 to limit unicast traffic received from AS1 to 100 pps.
-  Configure DS to limit broadcast traffic received from AS1 to 10Mbps.

