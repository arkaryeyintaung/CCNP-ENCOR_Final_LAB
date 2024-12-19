![image](https://github.com/user-attachments/assets/8e705ac3-2fe0-4b0b-8218-1af6c761db20)

<h1 align="center">Site-1 | Building-3 Diagram</h1> 

---

<h1 align="center">Task 3 Building 3</h1>

- Create VLANs on site1 switches according to diagram using VTP version 3.
- Ensure that only DS3 is in charge for vlan creation. Use VTP domain name “AMS” and password “AMSVTP!?” without quote.
- DS3 must have the least chance of being elected the root bridge for any vlans.
- Access-port must immediately transition to the forwarding state upon link up, as long as they do not receive a BPDU. Use the minimal number of commands per switch to enable this feature.
- If an access-port receives a BPDU, it must automatically shut down. Use the minimal number of commands per switch to enable this feature.
- DS3 must be the spanning tree root bridge and must maintain a single spanning tree instance for the following VLANs: 1006,1007 using instance 1.
- DS3 must be the spanning tree root bridge and must maintain a single spanning tree instance for the following VLANs: 1008,1009 using instance 2.
- Configure Layer 2 EtherChannel between DS3 and AS3 using static EtherChannel.
- Configure inter-vlan routing on DS3 so that all vlan can communicate each other.
- Configure the switches so that traffic between devices in all VLANs are tagged when sent over the trunk links.
- Configure ports Ethernet0/2 to E1/1 on AS3 to be access ports in respective VLAN.
- Configure DS3 so that STP logically blocks Ethernet links connected to AS3 if AS3 tries to become Root Bridge for any VLAN.

![image](https://github.com/user-attachments/assets/ba1a84ea-837c-4def-9443-df02c0269217)
