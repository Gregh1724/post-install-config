<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket -  Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source helpdesk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure
- Virtual Machine
- osTicket 


<h2>Good Things to Know</h2>

 - Click on specific positions for a better understanding!
 	- [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)
	- [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)
	- [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html) 
	- [Agents](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)
	- [Users](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html).
	- [Service Level Agreement(SLA)](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)
	
   

<h2>Installation Steps</h2>

<h3>Step 1: Open osTicket and Log In

- Log in to osTicket using the credentials you made during the installation tutorial </h3>
	- 

<p align="center">
<img src="https://i.imgur.com/mjE9FgF.png" height="80%" width="80%" alt="Azure Free Account"/>	


<h3>Step 2: Configure Roles </h3>

- Make sure you are in the Admin panel (check the top-right of the screen to see which panel you are in)
	- If it says "Agent," you are in the Admin panel
- Select the Agent tab > Roles > Add New Role
	- Name: Supreme Admin
	- Select Permissions tab and check every box under the "Tickets," "Tasks," and "Knowledgebase" sections
- Select Add Role
	
<p align="center">
<img src="https://i.imgur.com/2OFdViD.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/yysE1mg.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 3: Configure Departments</h3>

- Ensure you are still in the Admin panel
- Select the Agent tab > Departments > Add New Department 
	- Name: System Administrators
- Select Create Department 


<p align="center">
<img src="https://i.imgur.com/bS5FaEl.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/kw6Slek.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 4: Configure Teams
</h3>

- Select the Agent tab > Teams > Add New Team
	- Name: Level II Support 
- Go to the Members tab and select yourself in "Select Agent" dropdown menu
- Select Create Team
	
<p align="center">
<img src="https://i.imgur.com/OukSpkW.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/1t2urW9.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>

<h3>Step 5: Allow Anyone to Create Tickets</h3>

- Select Settings > User Settings
	- Make sure the following box is unchecked: 
		- Registration Required: Require registration and login to create tickets 
		
<p align="center">
<img src="https://i.imgur.com/akX1iB6.png" height="80%" width="80%" alt="Azure Free Account"/>		


<h3>Step 6: Configure Agents</h3>

- Select the Agent tab > Add New Agents
	- Name: Jane Doe
	- Email : jane.doe(@)osticket.com
	- Username: jane.doe
	- Click Set Password and uncheck the box that says "Send the Agent a Password Reset Email"
		- Set your password to anything you like
		- Uncheck the box that says "Require Password Change at Next Login"
		- Select set
		
<p align="center">
<img src="https://i.imgur.com/0Sk5Dwv.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/1yXxFpI.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>

- Select the Access tab 
	- Under Primary Department: 
		- Select the Department dropdown menu > System Administrators
		- Select the Role dropdown menu > Supreme Admin
	- Extended Accesss 
		- Select Department > Support > Add > Supreme Admin
- Select Team tab
	- Select Team dropdown menu > Level II Support
	- Select Add
- Select Create	

	
<p align="center">
<img src="https://i.imgur.com/jRPFNPY.png" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/BakdKm2.png" height="70%" width="70%" alt="Azure Free Services"/>
</p>

     
<h3>Step 7: Configure Users
</h3>

<p align="center">
<img src="https://i.imgur.com/OvrAzjj.png"80%" width="80%" alt="Azure Free Account"/>		
	
- Select the Users tab to create a user
	- Email Address: Karen(@)osticket.com
	- Full Name: Karen Karen
	- Select Add User
	
<p align="center">
<img src="https://i.imgur.com/mBR7HGM.png" height="80%" width="80%" alt="Azure Free Account"/>			
	
	
<h3>Step 8:  Configure Service Level Agreements (SLA)
</h3>

- We will create three SLAs
- Select the Manage tab > SLA > Add New SLA Plan
	- Name: SEV-A 			
	- Grace Period: 1
	- Schedule dropdown menu: 24/7
	- Select Add Plan
	
<p align="center">
<img src="https://i.imgur.com/GSR8evR.png" height="80%" width="80%" alt="Azure Free Account"/> <img src="https://i.imgur.com/bp74k9z.png" height="80%" width="80%" alt="Azure Free Services"/>
</p>
Repeat the steps to add SEV B and SEV C

	- Name: SEV-B
	- Grace Period: 4
	- Schedule dropdown menu: 24/7
	- Select Add Plan
	

        - Name: SEV-C 
	- Grace Period: 8
	- Schedule dropdown menu: Monday - Friday 8AM - 5PM with U.S. Holidays
	- Select Add Plan

<p align="center">
<img src="https://i.imgur.com/olp9LXQ.png" height="80%" width="80%" alt="Azure Free Account"/>



<h3>Step 9:   Configure Help Topics
</h3>

- We will create four Help Topics
- Select the Manage tab > Help Topics > Add New Help Topic
	- Business Critical Outage
	- Personal Computer Issues
	- Equipment Request
	- Password Reset
- Select Add Topic for each topic

<p align="center">
<img src="https://i.imgur.com/clsfQ4h.png" height="80%" width="80%" alt="Azure Free Account"/>



 We have configured osTicket succesfully! 
