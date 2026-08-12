# Home Network Segmentation Lab

## Project Overview

This project demonstrates the design and implementation of a segmented home network using VLANs, inter-VLAN routing, DHCP, ACLs, and network isolation.

The goal was to separate trusted devices, lab systems, and IoT devices into different network segments while maintaining internet connectivity and controlling communication between VLANs.

The lab was built using a TP-Link ER605 VPN router and a TP-Link SG2008 managed switch.

## Objectives

- Create multiple VLANs for different device groups
- Configure separate IPv4 subnets and DHCP scopes
- Configure tagged and untagged switch ports
- Assign PVIDs to access ports
- Configure inter-VLAN routing
- Restrict LAB access to the HOME network using an ACL
- Fully isolate the IoT VLAN from internal networks
- Validate segmentation using DHCP, ICMP, and internet connectivity testing
- Document troubleshooting and configuration results

## Hardware and Software

- TP-Link ER605 Gigabit VPN Router
- TP-Link SG2008 Managed Switch
- Windows 11 Desktop PC
- Windows Laptop
- PlayStation 5
- Ethernet cabling
- TP-Link web management interfaces
- Windows Command Prompt
- Windows PowerShell
- Windows Defender Firewall with Advanced Security

## VLAN and IP Addressing Plan

| VLAN | Name | Subnet | Gateway | DHCP Range | Purpose |
|---|---|---|---|---|---|
| 10 | HOME | 192.168.10.0/24 | 192.168.10.1 | 192.168.10.100-199 | Trusted personal devices |
| 20 | LAB | 192.168.20.0/24 | 192.168.20.1 | 192.168.20.100-199 | Lab and testing systems |
| 30 | IOT | 192.168.30.0/24 | 192.168.30.1 | 192.168.30.100-199 | IoT devices / future wireless access point |
