# NetCore Systems LTD. — Cisco Packet Tracer Network Configuration

## Project Overview

This project documents the design, configuration, and testing of a simulated corporate network for **NetCore Systems LTD.** using Cisco Packet Tracer.

The network includes separate IT, Sales, and Human Resources (HR) workstations, server infrastructure, router interfaces, Dynamic Host Configuration Protocol (DHCP) configuration, and Access Control List (ACL) rules to control selected traffic between departments.

The primary focus of the project is to configure network connectivity, automate IP address assignment, identify server infrastructure, and implement and test a traffic restriction that blocks ICMP echo traffic from the Sales department to the IT department.

## Objectives

- Build and document a corporate network topology in Cisco Packet Tracer.
- Configure router interfaces for network connectivity.
- Identify and configure IT and FTP server infrastructure.
- Configure DHCP for workstations in the IT, Sales, and HR departments.
- Implement an Access Control List to block ICMP echo traffic from Sales to IT.
- Test the ACL to verify the intended traffic restriction.
- Document the network configuration and testing process.

## Technologies and Tools

| Technology / Tool | Purpose |
|---|---|
| Cisco Packet Tracer | Network topology design, simulation, configuration, and testing |
| Cisco router | Network interface configuration and traffic routing |
| DHCP | Automatic IP address configuration for departmental PCs |
| FTP server | File Transfer Protocol server infrastructure |
| IT server | Server infrastructure for the IT environment |
| Access Control Lists (ACLs) | Filtering selected network traffic |
| ICMP | Network connectivity testing and echo traffic filtering |

## Network Architecture

The simulated network is organized around three departments and server infrastructure.

### Network Components

| Component | Role |
|---|---|
| IT department | Contains two workstations configured for DHCP |
| Sales department | Contains two workstations configured for DHCP |
| HR department | Contains two workstations configured for DHCP |
| IT server | Server component documented in the network configuration |
| FTP server | Server component documented in the network configuration |
| Router | Provides network interfaces for the simulated network |
| ACL | Blocks ICMP echo traffic from Sales to IT |

### Network Topology

The Cisco Packet Tracer topology serves as the foundation for the project. It connects the departmental workstations and server infrastructure through the configured network devices.

The accompanying assignment documents the topology, server IP configuration, FTP server, router interfaces, departmental DHCP configurations, ACL configuration, and ACL testing.

> **Note:** The exact IP addressing scheme, subnet masks, default gateways, VLAN assignments, router model, and interface names are not specified in this README because the available assignment text does not provide those values in a readable form.

## Implementation Details

### 1. Network Topology

The network topology was designed in Cisco Packet Tracer to represent the infrastructure of NetCore Systems LTD.

The design includes:
- IT, Sales, and HR departmental workstations.
- IT and FTP servers.
- A router with configured interfaces.
- Network traffic filtering using an ACL.

The topology provides the structure for configuring departmental IP addressing, routing, and traffic control.

### 2. Server Configuration

The project documents two server components.

**IT Server**
- The assignment includes a screenshot of the IT server's IP address.
- The server is part of the simulated corporate network infrastructure.

**FTP Server**
- The assignment includes a screenshot of the FTP server configuration.
- The FTP server represents the file transfer service component of the network.

The specific IP addresses, FTP settings, account credentials, and access permissions should be documented separately if they are available in the Packet Tracer configuration.

### 3. Router Interface Configuration

Router interfaces are documented as part of the network implementation.

The router configuration supports communication between connected network segments according to the topology and routing configuration.

The assignment includes a screenshot of the router interfaces. Exact interface names, IP addresses, subnet masks, and routing commands should be added from the actual Packet Tracer project.

### 4. DHCP Configuration

DHCP was configured for the workstations in all three departments so that the PCs could obtain their network settings automatically.

The assignment documents the following six workstations:

| Department | Workstation | Configuration |
|---|---|---|
| IT | PC1 | DHCP |
| IT | PC2 | DHCP |
| Sales | PC1 | DHCP |
| Sales | PC2 | DHCP |
| HR | PC1 | DHCP |
| HR | PC2 | DHCP |

DHCP reduces the need to configure each workstation manually and helps maintain consistent network configuration across the departmental PCs.

The assignment includes individual screenshots showing the DHCP configuration for each workstation.

**Suggested verification steps:**

1. Open each workstation in Cisco Packet Tracer.
2. Navigate to its IP configuration settings.
3. Confirm that DHCP is selected.
4. Verify that the workstation receives an IP address and other network parameters.
5. Record the assigned IP address, subnet mask, default gateway, and DNS server, where applicable.
6. Test connectivity to appropriate network destinations.

These verification steps describe how to validate the configuration; the assignment does not provide readable results for every individual test.

### 5. Access Control List (ACL) Configuration

An Access Control List was configured to block **ICMP echo traffic from the Sales department to the IT department**.

ICMP echo traffic is commonly associated with the `ping` command, which tests whether a destination is reachable over the network.

The intended security behavior is to restrict this specific type of traffic between Sales and IT while allowing other traffic according to the remaining network and ACL configuration.

The assignment documents:
- ACL configuration.
- Blocking ICMP echo traffic from Sales to IT.
- Testing the ACL after configuration.

The exact ACL type, rule sequence, source and destination IP addresses, wildcard masks, interface, and direction are not reproduced here because the corresponding commands and addressing details are not available as readable text in the document.

#### Expected ACL Behavior

| Test | Expected behavior |
|---|---|
| ICMP echo from Sales to IT | Blocked by the configured ACL |
| Other traffic between Sales and IT | Depends on the remaining ACL rules and network configuration |
| Traffic between other network segments | Depends on the configured routing and filtering rules |

The ACL should be evaluated against the intended policy and the actual configuration. Blocking ICMP echo does not, by itself, establish that all communication between Sales and IT is denied.

### 6. ACL Testing and Verification

The assignment includes screenshots documenting the ACL configuration, the ICMP echo restriction, and testing of the ACL.

A recommended verification process is:

1. Confirm that the relevant router interfaces are configured and operational.
2. Verify the IP configuration of the Sales and IT workstations.
3. Test the relevant destination from a Sales workstation using `ping`.
4. Confirm that ICMP echo traffic from Sales to IT is blocked as intended.
5. Test permitted traffic separately to determine whether the ACL affects only the intended traffic.
6. Review the ACL rules and interface placement if the results differ from expectations.
7. Record the results and supporting screenshots.

**Important:** A failed ping alone does not prove that an ACL is responsible. Incorrect addressing, missing routes, or other network conditions can also cause a ping to fail. Testing should confirm that the intended ACL is producing the observed behavior.

## Configuration and Testing Summary

The assignment documents the following implementation areas:

- [x] Cisco Packet Tracer network topology.
- [x] IT server IP configuration documentation.
- [x] FTP server configuration documentation.
- [x] Router interface configuration documentation.
- [x] DHCP configuration for IT PC1 and PC2.
- [x] DHCP configuration for Sales PC1 and PC2.
- [x] DHCP configuration for HR PC1 and PC2.
- [x] ACL configuration documentation.
- [x] ICMP echo restriction from Sales to IT.
- [x] ACL testing documentation.

These checkboxes indicate areas covered by the submitted assignment; they are not independent confirmation that every configuration has been validated in a live network.

## Skills Demonstrated

This project provides practical exposure to the following networking concepts:

- **Network topology design:** Representing a corporate network in a network simulation environment.
- **Router configuration:** Working with router interfaces as part of a multi-segment network.
- **IP addressing:** Examining server and workstation IP configuration.
- **DHCP:** Configuring automatic network addressing for multiple departments.
- **Server infrastructure:** Working with IT and FTP server components.
- **Network security:** Applying ACL-based traffic restrictions.
- **Connectivity testing:** Using ICMP echo behavior to assess network reachability.
- **Troubleshooting:** Comparing expected network behavior with test results.
- **Technical documentation:** Recording configurations and testing evidence with screenshots.

## Project Evidence

The original assignment contains screenshots covering the following areas. Add the corresponding images to the repository if you want them to appear directly in this README.

A suggested repository structure is:

```text
NetCore-Systems-Network/
├── README.md
├── packet-tracer/
│   └── netcore-systems.pkt
└── screenshots/
    ├── network-topology.png
    ├── it-server-ip.png
    ├── ftp-server.png
    ├── router-interfaces.png
    ├── it-pc1-dhcp.png
    ├── it-pc2-dhcp.png
    ├── sales-pc1-dhcp.png
    ├── sales-pc2-dhcp.png
    ├── hr-pc1-dhcp.png
    ├── hr-pc2-dhcp.png
    ├── acl-configuration.png
    ├── acl-icmp-block.png
    └── acl-testing.png
```

*The filenames above are suggested names for organizing project evidence. They do not indicate that those individual image files or the `.pkt` file are already included in the repository.*

## Future Improvements

Potential improvements to this project include:

- Documenting the complete IP addressing and subnetting plan.
- Recording the IP address, subnet mask, and default gateway of every workstation and server.
- Documenting the router interface configuration and routing commands.
- Including the exact ACL commands and explaining each rule.
- Recording successful and unsuccessful connectivity tests with their expected results.
- Documenting FTP access and testing, if FTP functionality is part of the project requirements.
- Adding the Cisco Packet Tracer `.pkt` file and supporting screenshots to the repository.
- Expanding the security configuration with additional controls appropriate to the network's requirements.

## Conclusion

The NetCore Systems LTD. Cisco Packet Tracer project documents a simulated corporate network with departmental workstations, server infrastructure, router interfaces, DHCP configuration, and ACL-based traffic filtering.

The project demonstrates foundational networking concepts, including automatic IP configuration, network connectivity, server configuration, and traffic restriction between departments. The documented ACL requirement focuses on blocking ICMP echo traffic from Sales to IT, with screenshots showing the configuration and testing process.

This project can serve as a portfolio example of hands-on networking practice and a foundation for further work in network engineering and cybersecurity.

## Author

**Gaspard Niyokindi**

University of Ottawa

**Areas of interest:** Network Engineering, Cybersecurity, and Governance, Risk, and Compliance (GRC).

---

*Project environment: Cisco Packet Tracer*  
*Project: NetCore Systems LTD. Network Configuration*

