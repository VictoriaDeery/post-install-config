<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket. This includes creating roles, a department, a team, users of the platform called agents, an enduser, SLA configuration for working with tickets, and help topics for endusers to categorize the tickets they create for the analysts or agents. 
<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation-coming soon](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles 
- Configure Departments and Teams
- Allow anyone to create Tickets
- Configure Agents (workers) and Users (customers)
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
  
- See first:
  - [Azure Compute and Networking](https://github.com/victoriadeery/azure-computing-and-networking),
  - [osTicket: Prerequisites and Installation](https://github.com/victoriadeery/osticket-prereqs), 
- Resources:
  - Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
  - End Users osTicket URL: http://localhost/osTicket 

<img src="https://github.com/user-attachments/assets/e4ae2fea-6a74-42ef-840b-9f00e7ec643b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
1. To configure roles: Use the Admin page to naviagate to click on "agents" in the top right. Then click on "roles" above"--All Teams--." Here can update role prmissions and create new roles by selecting "role" again and then "add new role" naming it, and selecting Permissions to define its permissions for tickets, tasks, and knowledgebase. For example a user called Supremem Admin that has access to all.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/fdfa597a-092a-45e0-bcc3-670270a2a70a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
2. To configure Departments: stay on the Admin Panel -> Agents -> Departments -> Add new department. Consider deleting the "Maintanance" Depatment as tickets get auto-assigned here. Otherwise select "Add new department" For example, you may now input "SysAdmins for Name and have them at the top level department so they may view all tickets in all departments. In the access tab, you may assign relevent agents, click the orange "create dept" button to create it. You may also want to delete the "Maintanance" Depatment as tickets get auto-assigned here. However, if you would like agents from different departments to work together, you may create a Team.

</p>
To configure a team: Admin Panel -> Agents -> Teams -> Add new department. For example call it "Online Banking" and click the orange "create team" button to create it.
<p>
  
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b24256e7-93e0-4f1c-861d-f77c9d2a2e2c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. To give everyone, even those without an account access to create a ticket: Admin Panel -> Settings -> Users -> Make sure "Require registration and login to create tickets" is Unchecked.

</p>
<br />
<p>
<img src="https://github.com/user-attachments/assets/481af333-ddab-4287-a6ce-3eb5e087ad7e" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4. To configure Agents (workers): Admin Panel -> Agents -> Add New Agent.
 For example add Jane Doe (Email: Jane@outlook.com; Username: Jane; Dept: SysAdmins; Role: Supreme Admin; Team: Online Banking) and John Doe(Email: John@outlook.com; Username: John; Dept: Support; Role: view only; Team: None Selected). To set the password for a user, on the account page select "set password", unselect "send the agent a password reset email" and input the password for the agent twice and select "update". To set the department and role select "access" and choose. And then select "teams" to put them on a team if desired. And lastly select "create" in orange.

<p>
<img src="https://github.com/user-attachments/assets/46600dbc-9531-4957-9f7f-caf5e5425ab4" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
5. To configure Users (customers): Agent Panel -> Users -> Add New -> Add new user. notice we are switching to the agent panel.

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/9b1e6013-7274-4ad4-b13f-210ee5b158d2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6. To configure SLA: Admin Panel -> Manage -> SLA -> Add New SLA Plan. Notice we are back in the admin panel. For example create the following SLAs:
  <p>
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
    </p>
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
</p>
Sev-C (Grace Period: 8 hours, Business Hours)
</p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/f95c8e34-f6b9-4563-81e9-583650b831bd" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7. To configure Help Topics: Admin Panel -> Manage -> Help Topics -> Add New Help Topic
  Help Topics are the category options for ticket creators to choose as the topic of their tickets. For example add "Business Critical Outage" and select "report a problem" for the parent topic and select the orange button "Add topic." Another Help topic you can add would be "Personal Computer Issues" (report a problem), "Equipment Request" (General Inquiry), "Password Reset" (report a problem), and "Other" (General Inquiry)
</p>
<br />
</p>
</p>
