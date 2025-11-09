<p align="center">
  <img src="https://raw.githubusercontent.com/tylergehm/post-install-config/main/osticketlogo.jpg" alt="GitHub banner" style="max-width:100%;height:auto;" />
</p>

<h1>osTicket - Post-Install Configuration</h1>
This Azure project focuses on configuring the osTicket helpdesk to simulate enterprise support operations. Using the Admin Panel, it sets up roles to group permissions, departments to manage ticket visibility, and teams to coordinate agents across departments. It enforces user registration for ticket submission, adds agents and users, defines SLA plans to enforce response times, and creates help topics to route incoming tickets—establishing a structured, role-based, and policy-driven support workflow within the previously deployed osTicket environment. </p>

For this project, the osTicket web portals will be used to log in as various roles: </p>

[Admin/Analyst Login Page:](http://localhost/osTicket/scp/login.php) - This is the staff portal where agents log in to manage, assign, and resolve tickets. </p>

[End User osTicket URL](http://localhost/osTicket) - This is the public help desk page where clients submit tickets and check ticket status.</p>

This project is created from the osTicket build completed in another project: [osTicket - Building osTicket Support Ticketing System from scratch](https://github.com/tylergehm/osticket-prereqs)

<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 11 Pro (21H2)
- Windows 11 Home (host machine)

<h2>Post-Install Configuration Steps</h2>

- Step 1 - Configure Roles
- Step 2 - Configure Departments
- Step 3 - Configure Teams
- Step 4 - Allow Ticket Creation
- Step 5 - Configure Agents (Employees)
- Step 6 - Configure Users (Customers)
- Step 7 - Configure Service Level Agreements (SLAs)
- Step 8 - Configure Help Topics

<h2> Step 1 - Configure Roles</h2>

<img width="1864" height="910" alt="image" src="https://github.com/user-attachments/assets/970dc40a-a015-499a-9cd9-bceaeef87ef6" /> </p>

The first step of this configuration begins by logging into the web portal with the admin account that was set up during osTicket installation </p>

<img width="1182" height="431" alt="image" src="https://github.com/user-attachments/assets/9f12f4f1-d5d9-4275-bc20-3585a5df03c9" />

Once logged into the Admin panel; click on the tab "Agents" then click on the tab "Roles". Once inside the Roles page, click the button that says "Add New Role". </p>

Roles are permission sets in osTicket that define what agents can do (e.g., view, edit, delete tickets or manage settings) without granting full admin access. </p>

<img width="1174" height="498" alt="image" src="https://github.com/user-attachments/assets/ae1349fe-f643-4ebe-bf26-940a01c65b67" /> </p>

Here, a new role is created with the name "Supreme Admin". Next, click the button labeled "Permissions". </p>

<img width="1037" height="681" alt="image" src="https://github.com/user-attachments/assets/f76aa8e8-7530-4bfd-b20e-dc034b634875" /> </p>

Inside the permissions tab, click the check-box next to all permissions to enable everything. This gives the Supreme Admin role access to all permissions. </p>

Permissions are specific actions (view, create, edit, delete, close tickets, manage users, etc.) that a role allows or denies—controlling exactly what an agent can do in osTicket. </p>

<img width="1150" height="510" alt="image" src="https://github.com/user-attachments/assets/4b47c900-8dcb-44b8-9be5-5203ddb1c8b8" /> </p>

The Supreme Admin role has been successfully added to the Roles manager. </p>

<h2>Step 2 - Configure Departments</h2>

<img width="1177" height="358" alt="image" src="https://github.com/user-attachments/assets/232815c9-5118-4e6e-8ad3-8eb5e1fceeab" /> </p>

To begin this step, click on the "Departments" button inside the Agents tab. </p>

Departments in osTicket are logical groups (like IT, HR, Billing) that organize agents and route tickets to the right team for faster, targeted support. It allows for ticket visibility, so Agents will see tickets that are relevant to their department.</p>

Click on the button labeled "Add New Department". </p>





