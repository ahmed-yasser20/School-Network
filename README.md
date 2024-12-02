School Network Project
Overview
This project involves designing and implementing a network for a school consisting of two buildings, each with three floors. The network is designed to provide connectivity, security, and scalability, ensuring smooth operation under all conditions.

Network Structure
Building Layout:
Each building has three floors, divided into two offices per floor.
Departments assigned to each floor:
1st Floor: Operations (VLAN 30).
2nd Floor: HR (VLAN 20).
3rd Floor: Teachers and Students (VLAN 10).
IP Allocation:
Each office is allocated a range of 50 IP addresses, ensuring adequate capacity.
Key Features
VLANs for Segmentation:

Separate VLANs for each department and floor for better management and security.
EtherChannel for Increased Bandwidth:

Implemented on Layer 2 switches to improve throughput and redundancy.
Port Security:

Applied to all Layer 2 switches to enhance security by restricting unauthorized device access.
Topology Design:

Focused on Integrity and Scalability:
Ensures continuous operation of unaffected devices during failures.
Allows seamless addition of new devices or offices in the future.
Dynamic IP Assignment:

Configured DHCP server to assign IP addresses dynamically to devices.
Domain Name Resolution:

Added a DNS server to translate domain names to IP addresses.
Time Synchronization:

Configured NTP server to synchronize time across all devices.
Log Management:

Integrated Syslog server to store logs for troubleshooting and monitoring.
DMZ and Web Server:

A DMZ was set up with a web server:
Assigned both a public IP for external access and a private IP for internal use.
Secured using a firewall.
PAT Configuration:

Implemented Port Address Translation (PAT) on the firewall:
Allows multiple private IPs to share a single public IP for internet access.
Dynamic Routing with OSPF:

Configured OSPF for efficient and scalable routing.
Technologies Used
VLANs: Network segmentation.
EtherChannel: Enhanced bandwidth and redundancy.
DHCP: Automatic IP allocation.
DNS: Domain name resolution.
Syslog: Log storage and monitoring.
NTP: Time synchronization.
PAT: Public-private IP translation.
OSPF: Dynamic routing.
Firewall: Network security and access control.
Goals
Provide a reliable and secure network infrastructure.
Ensure scalability for future expansions.
Enhance bandwidth and optimize resource utilization.
Maintain integrity during device or link failures.
How to Run
Open the project in Cisco Packet Tracer.
Test connectivity using:
Ping between devices in the same VLAN and different VLANs.
Access the web server using the public IP from an external network.
Simulate device failures to validate scalability and redundancy.
Future Improvements
Implement advanced monitoring tools.
Add a backup internet connection for redundancy.
Introduce advanced firewall rules for improved threat detection
