Windows Server 2022 Active Directory Home Lab
A hands-on home lab built with VMware Workstation 17, Windows Server 2022, and a Windows 11 client. This project demonstrates basic Active Directory organizational structure, user and group organization, DNS configuration, and joining a client computer to a domain.
Project objectives
- Create an Organizational Unit (OU) structure for a small company.
- Organize users, security groups, and computers into separate OUs.
- Configure a Windows 11 client to use the domain controller for DNS.
- Rename the client computer and join it to the pardhu.com domain.
- Document the setup as an IT Helpdesk / System Administration practice project.

- OU architecture
The Active Directory structure created for this lab is:
pardhu.com
└── my-ou
    ├── Computers
    │   └── CLINTComputer
    ├── Groups
    │   ├── Distro-group
    │   └── IT-group
    └── Users
        ├── Ajay DR
        ├── Kumar DR
        ├── Salma DR
        ├── Rahul IT
        ├── Sandhya IT
        └── Vijay IT

  Group membership
Groups
├── Distro-group
│   ├── Ajay DR
│   ├── Kumar DR
│   └── Salma DR
└── IT-group
    ├── Rahul IT
    ├── Sandhya IT
    └── Vijay IT
Work completed
1. Installed Windows Server 2022 in VMware Workstation 17.
2. Promoted the server to a domain controller for pardhu.com (from the earlier lab setup).
3. Used the server IP 192.168.211.139 as the DNS server for the Windows 11 client.
4. Created the parent OU my-ou.
5. Created three child OUs: Computers, Groups, and Users.
6. Created two groups in the Groups OU: Distro-group and IT-group.
7. Created six user accounts in the Users OU: Ajay DR, Kumar DR, Salma DR, Rahul IT, Sandhya IT, and Vijay.
8. Added Ajay DR, Kumar DR, and Salma DR to Distro-group.
9. Added Rahul IT, Sandhya IT, and Vijay to IT-group.
10. Installed Windows 11, renamed the client to CLINTComputer, and joined it to pardhu.com.
11. Placed the client computer object in the Computers OU.


