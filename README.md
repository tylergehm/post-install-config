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

<img width="792" height="923" alt="image" src="https://github.com/user-attachments/assets/61c0777e-fd39-470a-9546-2e5cb3aae28e" />

In the "Add New Department" page, the forms are filled out for a Top-Level Department with the name "Sys Admins" to be created. Once the forms are completed, click on the "Create Dept" button. </p>

<img width="1184" height="443" alt="image" src="https://github.com/user-attachments/assets/fa53aa9b-9876-4ff9-9c86-94473886dcdb" /> </p>

The "Sys Admins" department was successfully added to Departments. </p>

<h2Step 3 - Configure Teams</h2>

<img width="1182" height="326" alt="image" src="https://github.com/user-attachments/assets/aa794754-2802-4bc5-a6d1-93443dd4ceed" /> </p>

Under the Agents tab, click on the button labeled "Teams". Then, click on the button labeled "Add New Team" </p>

Teams in osTicket are flexible groups of agents (from any department) created for specific projects or situations. </p>

<img width="1035" height="804" alt="image" src="https://github.com/user-attachments/assets/1ffde357-e184-48b3-8397-24ef714084bb" /> </p>

Inside the Add New Team page, a team named "Online Banking" is entered into the text box. Afterwards, click the button labeled "Create Team" </p>

<img width="1179" height="350" alt="image" src="https://github.com/user-attachments/assets/fb6efcbe-d08c-4cef-a382-ab2a9180fad3" /> </p>

Online Banking has been successfully added to teams. </p>


<h2>Step 4 - Allow Ticket Creation</h2>

This next setting allows users to create tickets their own tickets even if they are not registered in the system yet. This allows for ticket creation without requiring an account. </p>

<img width="1179" height="812" alt="image" src="https://github.com/user-attachments/assets/d133f062-be40-4f99-ac68-63cf23aff7f7" /> </p>

Click on the "Settings" tab then click on the button labeled "Users". </p>

Inside the Users Settings, uncheck the box next to "Require registration and login to create tickets". </p>

Then click the button labeled "Save Changes".

<h2>Step 5 - Configure Agents (Employees)</h2>

<img width="1184" height="374" alt="image" src="https://github.com/user-attachments/assets/1b78745e-4cbc-499b-aff3-cb4458f0743d" /> </p>

To begin creating Agents, click on the "Agents" tab and then click on the button labeled "Add New Agent". </p>

Agents are staff members (support reps) who log into the osTicket admin panel to view, respond to, assign, and resolve tickets. </p>

<img width="1189" height="762" alt="image" src="https://github.com/user-attachments/assets/40749ab0-29e5-4f1f-b131-522cd479e59b" /> </p>

Inside the Add New Agents page; fill out the information for the new Agent including name, e-mail, and user name. Then click the tab labeled "Access". </p>

<img width="1180" height="638" alt="image" src="https://github.com/user-attachments/assets/af511f12-c06a-467b-85c4-2ed649241451" /> </p>

Set the Department and Role for the Agent being created, then click on the tab labeled "Teams". </p>

<img width="1193" height="512" alt="image" src="https://github.com/user-attachments/assets/cc608dc8-b56e-40c0-b187-564f165abcb6" /> </p>

Set the team the Agent will be assigned to, then click the button labeled "Create". </p>

<img width="1196" height="441" alt="image" src="https://github.com/user-attachments/assets/4d4c8174-de78-4833-bf18-68bcb27c4beb" /> </p>

Agent was successfully created. </p>


<h2>Step 6 - Configure Users (Customers)</h2>

<img width="1190" height="408" alt="image" src="https://github.com/user-attachments/assets/561f2d1d-1af3-4809-96ed-8643334c1262" />

To begin adding Users, open up the Agent panel of osTicket. </p>

Inside the Agent panel, click on the tab "Users then click on the button labeled "Add New User". </p>










