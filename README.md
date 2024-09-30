# VLAN-Based Network Configuration with Subnetting and Security

## Overview
This project showcases a network setup for a medium-sized company with departments segregated using VLANs. Subnetting is applied to manage IP addressing efficiently. The configuration ensures secure communication and proper management of network resources.

## Topology
- **VLANs**: HR, SOC, IT, Native (Loopback), Management (SVI)
- **Router**: R1 (Handling inter-VLAN routing and DHCP)
- **Switches**: S1, S2, Distribution Switch (Dis-S)
- **Devices**: PCs in each VLAN with dynamic IP assignment via DHCP.

## Objectives:
- Implement subnetting for different VLANs.
- Configure switches for VLAN segmentation.
- Secure network devices (passwords, SSH access, encryption).
- Configure the management VLAN for administration purposes.
- Apply DHCP for automatic IP allocation.

## Network Details:
### Subnetting (192.168.1.0/24): 
The network is divided into 8 subnets, with each VLAN occupying a unique subnet. 

For example:
- VLAN 10 (HR) - `192.168.1.0/27`
- VLAN 20 (SOC) - `192.168.1.32/27`
- VLAN 30 (IT) - `192.168.1.64/27`
- Management VLAN (SVI) - `192.168.1.128/27`

Complete subnetting details are in the [Network_Subnetting.txt](Network_Subnetting.txt) file.

### Address Table:
Refer to the [Addressing Table.pdf](Addressing%20Table.pdf) for complete IP address assignments.

### Network Topology:
Refer to the [Lab-1_Mohamed_Khaled.pkt](Lab-1_Mohamed_Khaled.pkt).

## Configuration Files:
- **Switch 1 (S1)**, **Switch 2 (S2)**, **Distribution Switch (Dis-S)**, and **Router 1 (R1)** configurations are available in the [My_Configuration.txt](My_Configuration.txt) file.

## Steps to Implement:
1. Set up VLANs on the switches.
2. Configure trunk ports for VLAN traffic.
3. Assign IP addresses and configure management VLANs on each switch.
4. Secure the devices using SSH, password encryption, and MOTD banners.
5. Configure inter-VLAN routing on the router.
6. Apply DHCP configuration on the router to assign IP addresses dynamically.

## **Contact**
For any questions or feedback, please contact:
- **Name**: Mohamed Khaled Mahmoud Sayed
- **Email**: Mo7ammad244@gmail.com

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
