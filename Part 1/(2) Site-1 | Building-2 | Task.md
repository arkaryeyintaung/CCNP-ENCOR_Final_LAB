
![image](https://github.com/user-attachments/assets/1d7c5958-6c87-435d-abce-fd6a118c45e1)


<h1 align="center">Site-1 | Building-1 Diagram</h1> 

---

<h1 align="center">Task 2 Building 2</h1> 

- Create VLANs on site1 switches according to diagram.
- Configure RSTP on DS2 and AS2. DS should be root switch using primary command.
- Configure Layer 2 EtherChannel between DS2 and AS2 using Cisco's proprietary protocol for negotiation.
- Only DS2 should actively negotiate the EtherChannel negotiation.
- DS1 should initiate 802.1q trunk negotiation.
- Configure inter-vlan routing on DS2 so that all vlan can communicate to each other.
- Configure the trunk encapsulation on DS2’s inter-switch links as static 802.1q.
- Configure the switches so that traffic between devices in VLAN 999 is not tagged when sent over the trunk links.
- Configure ports Ethernet0/2 to E1/1 on AS2 to be access ports in respective VLAN.
- Configure Spanning-Tree Port Fast on access ports so that access port does not have to wait for the Spanning-Tree listening and learning phases to begin forwarding and enable port security on access ports.
- Configure DS2 so that STP logically blocks Ethernet links connected to AS2 if AS2 tries to become Root Bridge for any VLAN.


![image](https://github.com/user-attachments/assets/7845dd25-2ef6-4d4f-9ce0-195d9e46a016)
