
<h1 align="center">Task 4 OSPF Routing Question</h1> 

- Configure OSPF using process ID of 10 on site 1 network as follows:
- Use area 0 between CS and R1, CS and R2.
- Use area 1 between CS and DS1.
- Use area 2 between CS and DS2.
- Use area 3 between CS and DS3.
- Use area 4 on CS, WAN-SW and R7.
- Use only interface-level commands on CS.
- Don't use interface-level commands on other devices.
- Ensure that LSA type 2 should not be seen on site 1 devices.
- Ensure that CS should detect R1 and R2 failure within 3 seconds.
- Configure authentication on CS and R1 using MD5 and key AMS FULL LAB for control plane security.
- Ensure that control plane is secure between CS and DS1 using strongest method using key-string "AMS FULL LAB" without quote
- Configure OSPF area 1, area 2, area 3 so that CS filters inter area and external routes out as they are sent from area 0 to these areas.
- Devices in these areas should still have reachability to routes external to the OSPF area 1, 2, 3.
- Configure R1 and R2 to originate an external default route as long as the static default route is installed in the routing table.
- CS prefer the R1 as primary exit point. If R1 or ISP3 fail, CS should use R2 as its secondary exit point.
- Configure CS to advertise the summary routes 10.0.0.0/22, 10.0.4.0/22, 10.0.8.0/22
- Configure on DS1, DSZ and DS3 so that OSPF Hello packets are not sent out the LAN segments without routers attached.
