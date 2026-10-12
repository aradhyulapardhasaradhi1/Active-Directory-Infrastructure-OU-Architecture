Windows Server 2022 Active Directory Home Lab
A hands-on home lab built with VMware Workstation 17, Windows Server 2022, and a Windows 11 client. This project demonstrates basic Active Directory organizational structure, user and group organization, DNS configuration, and joining a client computer to a domain.
Project objectives
- Create an Organizational Unit (OU) structure for a small company.
- Organize users, security groups, and computers into separate OUs.
- Configure a Windows 11 client to use the domain controller for DNS.
- Rename the client computer and join it to the pardhu.com domain.
- Document the setup as an IT Helpdesk / System Administration practice project.

  flowchart TD
    A["pardhu.com"] --> B["my-ou"]
    B --> C["Computers OU"]
    B --> D["Groups OU"]
    B --> E["Users OU"]
    C --> F["CLINTComputer"]
    D --> G["Distro-group"]
    D --> H["IT-group"]
    E --> I["Ajay DR"]
    E --> J["Kumar DR"]
    E --> K["Salma DR"]
    E --> L["Rahul IT"]
    E --> M["Sandhya IT"]
    E --> N["Vijay IT"]

  
