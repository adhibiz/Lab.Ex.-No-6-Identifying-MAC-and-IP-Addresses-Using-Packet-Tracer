# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date: 15/09/2025
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>
<img width="2878" height="1799" alt="image" src="https://github.com/user-attachments/assets/5c8ce2dd-0c49-4c7b-a2ad-2b8e87d862f6" />
<img width="2879" height="1471" alt="image" src="https://github.com/user-attachments/assets/326bfae7-8866-47dd-80c5-a20151ddc02e" />

<img width="2870" height="1236" alt="image" src="https://github.com/user-attachments/assets/5c9bc887-5b91-43fe-8b4c-aae7fb095648" />
<img width="2879" height="1279" alt="image" src="https://github.com/user-attachments/assets/f6691eb8-084e-445a-a1cd-413f632bd153" />





•	PDU details for remote communication<br>
<img width="2876" height="1364" alt="image" src="https://github.com/user-attachments/assets/9a19f40c-1afb-417e-b6cc-48b275a1a126" />
<img width="2879" height="1311" alt="image" src="https://github.com/user-attachments/assets/0c89e482-a1d7-4414-abc3-51f2dd105398" />



•	Tables showing MAC/IP changes through each device<br>
<img width="2879" height="1285" alt="image" src="https://github.com/user-attachments/assets/e24df8b2-8288-44f8-b1b1-38780efd6d88" />

<img width="2880" height="1800" alt="image" src="https://github.com/user-attachments/assets/c1173c8a-cd7c-40c5-8656-92a9910de815" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

