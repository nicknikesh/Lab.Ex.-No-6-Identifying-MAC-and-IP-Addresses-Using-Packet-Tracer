# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:19-09-2025
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
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082934" src="https://github.com/user-attachments/assets/db3eff1f-2bf7-4089-b985-e88d1c0a93c6" />
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082945" src="https://github.com/user-attachments/assets/3a7465c5-8001-4f03-a682-23f8901b1c0f" />
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082956" src="https://github.com/user-attachments/assets/0a2e7674-b17a-4e58-a671-b579fe531f68" />
<img width="1920" height="1080" alt="Screenshot 2025-09-19 083008" src="https://github.com/user-attachments/assets/f21fda95-fde7-402f-b924-1d20b425a857" />


•	PDU details for remote communication<br>
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082233" src="https://github.com/user-attachments/assets/0db8f9d3-2cf2-4f2f-9ace-4dda99639370" />
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082242" src="https://github.com/user-attachments/assets/1139781b-2a8a-45c8-af0e-524250234ae3" />
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082251" src="https://github.com/user-attachments/assets/bcb8c17b-c390-4d2d-8182-1719135be6e7" />
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082300" src="https://github.com/user-attachments/assets/c8444ff1-21df-41c3-aacd-db25f14161c7" />
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082313" src="https://github.com/user-attachments/assets/35393e3c-6be8-4494-9616-f7173979ee24" />
<img width="1920" height="1080" alt="Screenshot 2025-09-19 082328" src="https://github.com/user-attachments/assets/0c2ddf10-dc59-473d-9fc2-3a9c23c6871e" />
•	Tables showing MAC/IP changes through each device<br>
<img width="636" height="246" alt="Screenshot 2025-09-19 082419" src="https://github.com/user-attachments/assets/902b8689-ba4e-4076-b920-7406b0d6cede" />
<img width="640" height="262" alt="Screenshot 2025-09-19 082447" src="https://github.com/user-attachments/assets/2365d049-7904-45fb-9f57-d2bd848dc8c3" />


________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

