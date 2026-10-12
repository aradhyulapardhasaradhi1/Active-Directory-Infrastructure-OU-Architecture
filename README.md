# Active-Directory-Infrastructure-OU-Architecture

Welcome to the documentation for the pardhu.com domain infrastructure setup. This document outlines the Organizational Unit (OU) hierarchy, group memberships, user allocations, and client machine integration configured in the lab environment.

🏗️ 1. OU Architecture Overview

The primary container for this deployment is established directly beneath the domain root (pardhu.com). Inside my-ou, a structured sub-OU hierarchy separates administrative and organizational boundaries for computers, security/distribution groups, and user accounts.

pardhu.com (Domain Root)
└── my-ou
    ├── Computers
    ├── Groups
    └── Users


👥 2. Organizational Units & Object Breakdown

💻 A. Computers OU

Purpose: Houses all domain-joined workstation and server computer objects within the my-ou scope.

Registered Host:

Computer Name: CLINTComputer

OS: Windows 11 Pro / Enterprise

Network Configuration:

DNS Server IP: 192.168.211.139 (Active Directory Domain Controller / DNS Server)

Joined Domain: pardhu.com

🛡️ B. Groups OUdomain controller

Purpose: Contains security and distribution groups used for resource permissions and email distribution lists.

Configured Groups:

Distro-group: Distribution group intended for general organizational or mailing list purposes.

IT-group: Security group designated for IT infrastructure personnel and access rights.

👤 C. Users OU

Purpose: Contains all user employee objects categorized under their respective functional teams.

Group Membership Mapping:

Assigned to Distro-group:

Ajay DR 

Kumar DR 

Salma DR 

Assigned to IT-group:

Rahul IT 

Sandhya IT 

Vijay IT 

⚙️ 3. Client Configuration Summary

To successfully join CLINTComputer the pardhu.com domain and place it inside the target OU, verify that the following prerequisites were met during setup:

DNS Pointing: The network adapter IPv4 properties CLINTComputer must explicitly point its Preferred DNS Server to the Domain Controller IP: 192.168.211.139.

Domain Join Credentials: Joined using an account with administrative privileges in pardhu.com.

Computer Account Verification: Verified that it is CLINTComputer successfully registered inside the Computers OU.
