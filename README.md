<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Roles
- Departments
- Teams
- Allow creation of Tickets
- Agents
- Users
- SLA
- Help Topics

<h2>Configuration Steps</h2>

<strong>Step 1:</strong> Setting up <a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">Roles</a>

<p>
Roles are permissions granted to Agents for each department they have access to. Each Role has it's own permissions that can be granted/denied for Agents
  who have that Role in association with deparments they have access to.
<br />
<br />
To start off we will create a role named "Supreme Admin" 
<br />
<br />
In the permissions tab just check mark everything, but take a moment to observe the multiple permissions roles can be assigned.
<br />
<br />
(Admin Panel) Agents ⇒ Roles
</p>

<p>
<img src="https://i.imgur.com/dI9jwGF.jpg" height="80%" width="80%" alt="Permissions"/>
</p>

<p>
<img src="https://i.imgur.com/bViS5hZ.jpg" height="80%" width="80%" alt="Setting Roles"/>
</p>

<br />
<br />
<br />

<strong>Step 2:</strong> Setting up <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">Departments</a>
<p>
Tickets are routed through Departments and there are many settings that can be set for each Department (Check documentation).
<br />
<br />
After creating a Role, right next to it is the Departments tab which we will be utilizing for this step.
<br />
<br />
Create a new Department named whatever you'd like, but for this example I will use "Systems Admin", leave everything else as default settings.
<br />
<br />
Take a minute to observe all the fields in each section of adding a new department
<br />
<br />
(Admin Panel) Agents ⇒ Departments
</p>
<p>
<img src="https://i.imgur.com/Kkxhu6V.jpg" height="80%" width="80%" alt="Added Department"/>
</p>
<p>
<img src="https://i.imgur.com/THPbO7c.jpg" height="80%" width="80%" alt="Added Department"/>
</p>

<br />
<br />
<br />

<strong>Step 3:</strong> Setting up <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">Teams</a>
<p>
Teams allow the use of pulling Agents from different departments to organize them to handle spcific issues via Help Topic or Ticket Filter.
<br />
<br />
Add a new Team and name it whatever you'd like, for this example I will add "Level II Support" since level I is created by default.
<br />
<br />
(Admin Panel) Agents ⇒ Teams ⇒ Add New Team
</p>

<p>
<img src="https://i.imgur.com/NFMEMec.jpg" height="80%" width="80%" alt="Adding Team"/>
</p>

<br />
<br />
<br />

<strong>Step 4:</strong> Allowing any user to create a ticket 
<p>
Here we are going to allow any user to create a Ticket. Generally registration can be required for Users to create tickets. This is done to prevent random tickets
  or limit accessibility to the help desk on the user's end.
<br />
<br />
Double check 'Require registration and login to create ticekts' is unchecked (This should already be done by default)
<br />
<br />
(Admin Panel) Settings ⇒ Users
</p>

<p>
<img src="https://i.imgur.com/zesopGu.jpg" height="80%" width="80%" alt="Authentication Settings"/>
</p>

<br />
<br />
<br />

<strong>Step 5:</strong> Setting up <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">Agents</a>
<p>
Agents have access to Helpdesk with the intention of responding and resolving tickets. Agents may have one to many departments and roles associated with one another.
<br />
<br />
We will be adding two Agents and giving them any name (I will use "Tim" and "Eric"), and take a moment to observe through the tabs 'Acess', 'Permissions', 'Teams'<br />
Next to the Username field, in Account; is set password. Click that and make sure the boxes are unticked and then create a password (we will be using these later)  
<br />
<br />
Access: Give them a department and role and any extended access<br />
Permissions: Check any permissions you would like<br />
Teams: Assign any team you'd like (You'll only see Level I Support & Level II Support or whatever you named the team in Step 3)
<br />
<br />
(Admin Panel) Agents ⇒ Agents
</p>

<p>
<img src="https://i.imgur.com/aQf7i7u.jpg" height="80%" width="80%" alt="Set Password"/>
</p>

<p>
<img src="https://i.imgur.com/Nq2p3gJ.jpg" height="80%" width="80%" alt="Set Access"/>
</p>

<p>
<img src="https://i.imgur.com/58BMCrE.jpg" height="80%" width="80%" alt="Set Permissions"/>
</p>

<p>
<img src="https://i.imgur.com/a0MYtMn.jpg" height="80%" width="80%" alt="Set Teams"/>
</p>

<br />
<br />
<br />

<strong>Step 6:</strong> Setting up <a href="https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html">Users</a>
<p>
Users (customers) can create an account and log in to create a ticket or check on their ticket status as well.
<br />
<br />
For this example we will create our users. Use any name (for this example I will use "Karen" and "Ken")
</p>
