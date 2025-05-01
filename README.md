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
- Agents
- Users
- Service level agreements
- Help topics

<h2>Configuration Steps</h2>


![image](https://github.com/user-attachments/assets/6639bf9f-ad60-4e9f-946f-7f4473c75087)


With osTicket being fully installed, you can now facilitate administrative tasks within the osTicket system. You should begin by creating "Roles" within the help desk. To configure roles within help desk, go to the Admin Panel > Agents > Roles. Select “Add new role”.


![image](https://github.com/user-attachments/assets/aa80a9c2-f034-47f1-9070-1d70cca1457c)

![image](https://github.com/user-attachments/assets/f6c68b8d-5a88-45f9-af36-01844fbb0b6e)


For the time being, you can create a "Supreme Admin" role to give complete access to the full osTicket system by selecting the necessary permissions and selecting "Add role".
</p>
<br />


![image](https://github.com/user-attachments/assets/2836d388-b593-4bb9-a961-2f71b56c0cc3)


Now, configure a new department. This promotes ticket visibility to certain roles such as sys admins, support etc. You can also configure other settings such as assigning agents and other possibilities.

![image](https://github.com/user-attachments/assets/13a6e075-3822-44d9-9e46-71589c9527c1)


Continue and create a "Team". The purpose of teams is to pull a group of agents from different departments. Navigate to Admin Panel > Agents > Teams. Create a team called “Tier 2 support” and select "create team".


![image](https://github.com/user-attachments/assets/904e4b20-6a9e-4b5c-8b13-bb6b4766df88)


Now to allow anyone to create tickets navigate to Admin Panel > Settings > User Settings. Ensure that the box for "Require registration and login to create tickets" is unchecked. Save changes.


![image](https://github.com/user-attachments/assets/c7309625-ad76-46e9-8b1b-d58ae3569c88)

![image](https://github.com/user-attachments/assets/08f13d17-42f6-48bb-879e-d91a159cc524)

![image](https://github.com/user-attachments/assets/e82a6b69-c3ed-4380-9872-d2e4466bbc68)


To be able to work on tickets "Agents" need to be created. Navigate to Admin Panel > Agents > Add New Agent. Enter the appropriate details for each agent, including their name, email address, assigned role and department. This will set up each agent’s profile and appropriate permissions.


![image](https://github.com/user-attachments/assets/e3be74e1-b1dd-4ae8-8d78-c509943019fc)


For the purpose of this project, you need to create users (also known as customers). Navigate  to the Agent Panel > Users > User Directory > Add User. Enter approprite details for the individual user. In this case, "John James" was created as a user.


![image](https://github.com/user-attachments/assets/e8e03b88-2fb5-481a-adb4-e664f012b1c1)


Next, configure SLA plans. Navigate to Admin Panel > Manage > SLA. SLAs (Service Level Agreements) are used to help prioritize tickets and to create "targets" for resolving the issue. For example: How quickly you reach out to a user, how often you communicate with them, and how quickly the issue is resolved. There can be levels of SLAs created which can pair with certain grace periods to complete.


![image](https://github.com/user-attachments/assets/011aa15d-3caa-4c91-a73c-f58af9226a52)

![image](https://github.com/user-attachments/assets/6d46c7f2-8dc1-4fad-a12f-520c6b8d4a7b)


To assist users in creating tickets, it’s helpful to configure help topics. Navigate to Admin Panel > Manage > Help Topics. The help topics we add can then be used as a guide to users in categorizing their tickets more effectively. In this case, "Equipment requests" was created. 
