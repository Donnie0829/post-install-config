 
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
  

  <h1>osTicket - Post-Install Configuration</h1>
  This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)



<h2>Configuration Steps</h2>


Step 1: Configure Roles

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Roles -> Add New role
- Add Name (Supreme Admin)
- Click the 'Permissions' tab and Check all boxes under Tickets\Tasks\Knowledgebase
- Click Add Role


![image](https://github.com/user-attachments/assets/debdbfb6-ea9f-4767-b6aa-68c009e505a2)

![image](https://github.com/user-attachments/assets/6584fe3c-7f41-4200-b950-e3a6ac87cf2b)

![image](https://github.com/user-attachments/assets/89d08018-3adb-4b0c-a823-cdac556a5960)



Step 2: Configure Departments

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Departments
- Click 'Add New Department'
- In the name field enter 'System Adminstrators'
- Click 'Create Dept' at the bottom of the webpage



![image](https://github.com/user-attachments/assets/05568987-7ce4-4f03-b2c4-257c8d0713d0)

![image](https://github.com/user-attachments/assets/fe908923-2d80-4bdd-b634-e7d51f6c530c)



Step 3: Configure Teams

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Teams
- Click 'Add New Team'
- In the name field enter 'Level II Support' (Note: There should already be a 'Level I Support' team there)
- Click the 'Members' tab and add yourself to the team
- Click 'Create Team' at the bottom of the webpage


![image](https://github.com/user-attachments/assets/8b19f973-23bd-4870-8e00-ff219fc1c9f2)

![image](https://github.com/user-attachments/assets/9d2fc25e-2519-43ae-8dc2-34d8a2da1873)



Step 4: Configure to allow anyone to create tickets

- Ensure you're under Admin Panel (top right should say Agentr Panel, which means you're in the 'AdminPanel') -> Settings -> Users -> Settings
- Make sure the 'Require registration and login to create tickets' box is unchecked

  ![image](https://github.com/user-attachments/assets/244a6403-83d6-40dc-8927-79c0fc0b0171)



  Step 5: Configure Agents (Help Desk Professionals)

  - Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') ->Agents -> Add New Agent
  - Add Agents Name\ Email Address\ Username
  - Click 'Set Password' and deslect 'Send the agent a password reset email'
  - Enter the password (create your own) -> deselect 'Require password change at next login' -> click 'set'
  - Assign the department for the agent by clicking the 'Access ' tab
  - Click 'Create'
  - Repeat steps to add a second agent
  - Assign the second agent to the 'Support' department and 'View Only' role under the 'Access' tab

![image](https://github.com/user-attachments/assets/76d33da5-1847-4055-ac51-21a4433fd3e6)

![image](https://github.com/user-attachments/assets/e537a660-de03-4a2d-9dc8-e2421596797c)

![image](https://github.com/user-attachments/assets/286123d5-b416-4f2c-ab46-06325529b2a8)

![image](https://github.com/user-attachments/assets/ef1af8e8-be76-4b5a-ad04-322313da0eaf)

![image](https://github.com/user-attachments/assets/904d0fb0-e44f-43b5-a72c-5cfdbf674420)



Step 6: Configure Users (Customers)

- Switch to the Agent Panel (top right should say Admin Panel, which means you're in the 'Agent Panel') -> Users -> Add User
- Enter a made up email address and name -> Add User
- Go back to the 'User Directory' and add a second user by repeating the exact same steps


![image](https://github.com/user-attachments/assets/ed9f16f8-9e8d-4de6-a75f-bd2104b45765)

![image](https://github.com/user-attachments/assets/1b3713da-23df-4f00-837c-35fb7bcb37f8)



Step 7: Configure SLA

- Switch back to the Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Manage ->SLA
- Click 'Add New SLA Plan'
- Add SEV-A (Grace Period: 1 hour) (Schedule; 24/7)
- Add SEV-B (Grace Period; 4 hours) (Schedule:24/7)
- Add SEV-C (Grace Period: 8 hours) (Schedule: Business Hours M-F)
- Click 'Add Plan' at the bottom of the webpage

![image](https://github.com/user-attachments/assets/a8632101-5d2e-44be-84de-1dc00e0293a1)

![image](https://github.com/user-attachments/assets/654b8d55-9202-4da6-bd7e-dda2f0befcd8)

![image](https://github.com/user-attachments/assets/8a2df2d9-d49e-4814-a612-b00b7ae3db82)



Step 8: Configure Help Topics

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Manage -> Help Topics
- Click 'Add New Help Topic'
- The following topics:
  - Business Critical Outage
  - Personal Computer Issues
  - Password Reset

 ![image](https://github.com/user-attachments/assets/52c24f2b-c5c5-4f91-8956-457bcda9f131)

 ![image](https://github.com/user-attachments/assets/9ea1e53e-38f9-4866-b785-afc7f8ea4ba4)

 ![image](https://github.com/user-attachments/assets/dfbc713a-c462-458e-9a63-0d550450ab88)

 ![image](https://github.com/user-attachments/assets/2c024a57-7ce9-4668-bf2f-91e05573f560)

 ![image](https://github.com/user-attachments/assets/453ff7ef-20ac-4023-893d-2edd1fa275fc)

 ![image](https://github.com/user-attachments/assets/3557e1ee-ed05-48bb-bb7e-8d97a6bff1f1)



 Congratulations, you have configured all os the core settings to create and work tickets in osTickets!



































