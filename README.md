<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post Configuration Setup</h1>
</p>
In this tutorial I will demonstrate the post configuration setup of the osTicket system .<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure 
- Remote Desktop
- osTicket
- Windows 10
<p>


## Post Config Setup Stages
</p>
</p>
<p>
Now that we have succesfully configured osTicket.
  
first order of business is to configure new roles within the help desk. In order to do this you will need to first go to the  Admin panel-> Agents-> Roles. From here we will create a new role called the Supreme Admin. 
Click on "Add new role" then enter the name of the new role. While doing this you can also edit any specific roles/permissions. Because we are creating a Supreme Admin we are going to give them permission on everything. 
For the future when creating roles you want to remeber that roles are used to detemine a agent users permissions, not all agents will need unlimited access like the Supreme Admin.
If you followed the steps correctly above your screen should like like this, and you will have succesfully created the "Supreme Admin" role.
</p>

![image](https://github.com/user-attachments/assets/da1a97c3-9c24-455e-8430-4865cf357c73)

</p>
<br />
<p>
</p>
<p>

Now we will create departments to help with ticket visability so that certain departments can see their own tickets.    
First thing you will do is select the "Departments" button in the agents tab. Once you do that you will be able to create a new department. Every agent is assigned to a department depending on their assigned role inside the helpdesk. For this tutorial we will be creating the "SysAdmins" department, this is where the Supreme Admins will be designated. Other specific settings such as SLAs, managers, and other email settings can be set up in the departments tab. However we will leave those blank for now.
</p>
<br />
<p>

![adding departments](https://github.com/user-attachments/assets/395e3ffe-ceee-4eb5-a470-bf4cfedf27e9)

If done correctly you will see your new SysAdmin department appear in your departments dashboard just like it does in the picture below

![department created correctly](https://github.com/user-attachments/assets/36d45dab-8b28-4e2d-bda2-ab8a1fb47ba2)


</p>
<p>
Now that we have configured a new department we will need to set up a new team as well. The purpose of teams is if you wanted to create a group of people who are all from different departments these teams can consist of many different people from SysAdmins to help desk professionals 
</p>
<br />
<p>

  ![creating a team](https://github.com/user-attachments/assets/11e54a15-c990-4fe0-8855-2eceda6e21a2)

</p>
<p>
The next step will be to create a new setting that will allow anyone to create tickets. Even if they arent registered in the system. To do this you will go to Admin Panel->Settings->User Settings. Once you get into the user settings you will make sure the box highlighted below is unchecked and save your changes. Now anyone can create a ticket 
</p>
<br />

![anyone can create a ticket](https://github.com/user-attachments/assets/0f314071-3c12-4ef3-b684-d1b810734c59)


</p>
<p>
It is now time to create Agents. These are employees of the help desk that help with resolving tickets. We will create two agents a Jane Doe and a John Doe. Agents will also be assigned primary departments, as well as be given a primary role for tickets sent to their department. Agents can be given access to other departments other than their own, you can do this by clicking the "Access" tab in the Manage agents dashboard. I have also included a picture highlighting the tab below 
</p>
<br />

![proof of two agents](https://github.com/user-attachments/assets/d60ea51c-9841-459c-8e41-1f3702a6a82e)

![agents dash](https://github.com/user-attachments/assets/a530b63f-8673-4893-9d43-a88b125068ab)




</p>
<p>
Now we will create users. Users are simply customers that may create tickets when they are having problems. To create a user you will click Agent Panel its in orange lettering at the top right hand section of your screen then you with click ->Users->User Directory->Add new. 
</p>
<br />

![creating users](https://github.com/user-attachments/assets/459e5d56-0e11-430e-a37a-02454513bd8a)


</p>
<p>
Now we will configure our SLAs. SLAs basically outline a certain amount of time in which help desk is expected to take to respond/resolve the ticket. Depending on severity of the issue it could be anywhere from 1 hour to 24 hours for  a specific ticket. 
SLA Plans are created by going to Admin Panel this is the orange lettering up in the upper right hand corner of the screen again. 
From there you will click ->Manage->SLA->Add New SLA Plan. Each SLA has a schedule and within that schedule there is a grace period. 
</p>
<br />

![seva](https://github.com/user-attachments/assets/066d73e0-3f29-4f73-a0ee-2e7cab38c60b)

We will create 3 SLA plans for SEV-A , SEV-B, And Sev-C all varying in expected response time and grace period to signify different levels of urgency needed to complete the ticket 

![3 sevs](https://github.com/user-attachments/assets/00682d5c-0495-4d5b-81ef-3da90d2e1e44)


<p>
Finally we will configure Help topics. 
To add a help topic you will click -> Manage ->Help Topics->Add New Help Topic
</p>
<br />

![help topics](https://github.com/user-attachments/assets/818a768f-f5b1-4e8e-ab61-9338db23108a)


In the example below we have made a few different help topics
to help users categorize their tickets. 

![list of help topics](https://github.com/user-attachments/assets/a1be271b-94c2-44a2-ba94-34ed44bf06fb)

</p>
<p>
