Windows Server 2022 Active Directory Home Lab
A hands-on home lab built with VMware Workstation 17, Windows Server 2022, and a Windows 11 client. This project demonstrates basic Active Directory organizational structure, user and group organization, DNS configuration, and joining a client computer to a domain.
Project objectives
- Create an Organizational Unit (OU) structure for a small company.
- Organize users, security groups, and computers into separate OUs.
- Configure a Windows 11 client to use the domain controller for DNS.
- Rename the client computer and join it to the pardhu.com domain.
- Document the setup as an IT Helpdesk / System Administration practice project.

  <img width="3110" height="952" alt="mermaid-diagram" src="https://github.com/user-attachments/assets/1c3a1979-0e4c-4915-8884-5a1bc82f8fc7" />

  
Group membership
This diagram shows group membership separately from OU placement. User accounts remain in the Users OU; being a member of a group does not move the user object into the Groups OU.

<img width="706" height="1152" alt="mermaid-diagram (1)" src="https://github.com/user-attachments/assets/f475b889-647f-4a2c-8834-72eb689037a1" />

Work completed
Created the parent OU my-ou.
Created three child OUs: Computers, Groups, and Users.
Created two groups in the Groups OU: Distro-group and IT-group.
Created six user accounts in the Users OU: Ajay DR, Kumar DR, Salma DR, Rahul IT, Sandhya IT, and Vijay.
Added Ajay DR, Kumar DR, and Salma DR to Distro-group.
Added Rahul IT, Sandhya IT, and Vijay to IT-group.
Installed Windows 11, renamed the client to CLINTComputer, and joined it to pardhu.com.
Placed the client computer object in the Computers OU.




