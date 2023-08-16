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

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Internet Information Services (IIS)
- PHP Manager
- Rewrite Module
- VC Redist
- MySQL
- Heidi SQL
- osTicket v1.15.8
  
- Link to downloads: https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>
1. Complete steps laid out in osTickets: Prerequisites and Installation
<p>

  ![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/7bf7bb3b-090a-4e8c-abc7-40ce85c7b1bb)

</p>
<p>
2. 
  Sign back into your Remote Desktop using the public IP Address found in your virtual machine 
</p>
<br />
3. If need be, sign back into http://localhost/osTicket/scp/login.php using same username and password as before. 

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/8d1b845c-c19f-4d62-ba7c-c5f42c592707)

<p>
4. Configure Roles: Admin Panel -> Agents -> Roles. 


</p>
5. Add a new role named Supreme Admin. Inside Permissions, check all boxes in Tickets/Task/Knowledgebase then click add role.
<p>
6. Configure Departments: Select Departments -> Add New Department. Name that System Administrators (Leave all other boxes as is) then clcik create. 
  
![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/a894b325-510e-49ec-882e-344403d00d83)

</p>
7. Configure Teams:
Admin Panel -> Agents -> Teams. 

Click Add New Team

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/0579ea7a-e4b9-4d05-8d25-545b7a2a1c5b)

8. Name  Level II Support. Go to Members, add your self (Sierra Miike) to team then click Create Team 

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/0eef51d9-40f8-4c5c-8bda-d1060e3228d5)

9. Allow anyone to create tickets: Admin Panel -> Settings -> User Settings. All your doing here is ensuring "Registration Required" is NOT SELECTED

   ![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/9fa51e74-1a96-45f5-b56f-fbed49f977c7)


10. Configure Agents (workers): Admin Panel -> Agents -> Add New (Jane, John)

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/b0affcb0-a28c-40c4-8055-f876c261311c)

11. Click "Set Password" next to username. Deselect Boxes, set parrword to Password1 then press set
12. In the Access tab, select roles as depicted. In Teams tab assign Jane to Level II Support Team, Click Create. 

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/260c2091-8799-4d62-9cd3-23322385f947)

13. Add another Agent (John Doe). Give John Doe same password following same instructions as in step 11.
14. In Access tab only give John Support and view only roles then create.  

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/c0d42873-3470-41a9-9e60-5182b637b10d)

15. Configure Users (customers): Agent Panel -> Users -> Add New Karen Ken

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/a2a83483-d10f-48b2-b731-41f57ca7b76d)

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/5ffe9929-8ee9-44ea-a80b-8bb1b922902a)

 16. Create another User named Ken repeating step 15
 17. Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (1 hour, 24/7)
Sev-B (4 hours, 24/7)
Sev-C (8 hours, business hours)

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/4ef57198-0418-4e26-a9ed-981794c6538d)

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/5159f736-6fc5-477f-aec5-5267ed9b46ab)

18. Configure Help Topics
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset

![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/b57eb191-5c0d-42b7-ba98-b4f228a23510)
Create ahelp topic for each of the 4 topiccs as depicted below.
![image](https://github.com/SeanMcClendon/post-install-config/assets/142221948/08d4e564-9f7e-4980-ad02-db9bee8627ce)


<h1>CONGRAUALTIONS YOU'RE FINISHED</h1>

<br />

<p>

</p>
<p>

</p>
<br />
