# Wireless LAN Controller (WLC) Network Project

## Project Title

**Enterprise Wireless Network Implementation Using Cisco Wireless LAN Controller (WLC) in Cisco Packet Tracer**

## Project Overview

This project demonstrates the design and implementation of a centralized wireless network using a Cisco Wireless LAN Controller (WLC). The network consists of one server, one Layer 2 switch, one Wireless LAN Controller, one management PC, one wireless laptop, and four departments: Sales, Human Resources (HR), Information and Communication Technology (ICT), and Finance.

The WLC provides centralized management of wireless devices, while VLANs are used to separate departmental traffic for improved security and performance.

## Objectives

* Design a centralized wireless network using a Cisco WLC.
* Create separate VLANs for each department.
* Enable communication between wireless clients and the server.
* Demonstrate secure and efficient wireless network management.
* Implement departmental network segmentation.

## Network Topology

The network includes the following devices:

* 1 Cisco Wireless LAN Controller (WLC)
* 1 Cisco Switch
* 1 Server
* 1 Management PC
* 1 Wireless Laptop
* Sales Department PCs
* HR Department PCs
* ICT Department PCs
* Finance Department PCs

### Department Allocation

| Department | VLAN    | Devices       |
| ---------- | ------- | ------------- |
| Sales      | VLAN 10 | PCs           |
| HR         | VLAN 20 | PCs           |
| ICT        | VLAN 30 | PCs           |
| Finance    | VLAN 40 | PCs           |
| Management | VLAN 50 | Management PC |
| Wireless   | VLAN 60 | Laptop        |

## IP Addressing Scheme (Example)

| Device/Department | Network          |
| ----------------- | ---------------- |
| Sales             | 192.168.10.0/24  |
| HR                | 192.168.20.0/24  |
| ICT               | 192.168.30.0/24  |
| Finance           | 192.168.40.0/24  |
| Management        | 192.168.50.0/24  |
| Wireless          | 192.168.60.0/24  |
| Server            | 192.168.100.0/24 |

## Hardware Used

* Cisco 2960 Switch
* Cisco Wireless LAN Controller (WLC)
* Generic Server
* Desktop PCs
* Laptop
* Copper Straight-through Cables

## Configuration Summary

### Switch Configuration

* Configure VLANs 10, 20, 30, 40, 50, and 60.
* Assign switch ports to the appropriate VLANs.
* Configure the port connected to the WLC as a trunk port.

### Wireless LAN Controller Configuration

* Assign a management IP address.
* Configure WLAN (SSID).
* Associate the WLAN with the Wireless VLAN.
* Configure DHCP relay or connect to the DHCP server.
* Enable wireless security (WPA2-PSK or WPA2 Enterprise if supported).

### Server Configuration

The server provides:

* DHCP services
* DNS services
* Web services (optional)
* File sharing (optional)

### Management PC

The Management PC is used to:

* Access the WLC web interface
* Monitor the wireless network
* Perform administrative tasks

### Wireless Laptop

The laptop:

* Connects to the configured SSID.
* Receives an IP address automatically from the DHCP server.
* Communicates with the server and other permitted network devices.

## Testing Performed

The following tests were completed successfully:

* VLAN connectivity verification
* Wireless client association
* DHCP IP address assignment
* Ping between wireless laptop and server
* Ping between management PC and WLC
* Departmental network isolation
* End-to-end connectivity testing

## Expected Results

* All wired devices communicate within their assigned VLANs.
* The wireless laptop successfully connects through the WLC.
* The server provides network services to authorized devices.
* Departmental traffic remains isolated using VLANs.
* The Management PC successfully manages the Wireless LAN Controller.

## Advantages of the Design

* Centralized wireless management
* Improved security through VLAN segmentation
* Easier network administration
* Scalable enterprise network design
* Reduced configuration complexity for wireless devices

## Conclusion

This project demonstrates the implementation of a centralized enterprise wireless network using a Cisco Wireless LAN Controller in Cisco Packet Tracer. The use of VLANs provides logical separation between departments, while the WLC simplifies wireless network management. The design offers improved scalability, security, and reliability suitable for a small or medium-sized enterprise.
