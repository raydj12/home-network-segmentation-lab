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
