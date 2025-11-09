<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
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
