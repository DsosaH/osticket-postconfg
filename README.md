<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-installation Configuration</h1>
This is the next part of the tutorial, where we'll configure osTicket so it is functional.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure 
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
<h2>Configuring Roles</h2>
<p>
  osTicket, like most ticketing systems, depend on a hierarchy in order to correctly deliver the ticket depending on how urgent and difficult a task is. For this reason, we need to create and assign the correct roles.<br>
  To begin, we need to first access to osTicket using the user we designated as our Admin. Once inside, we'll need to go to the Admin Panel in order to make changes.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/3196807e-740b-4e8b-9f25-176ad76fc904)

</p>
<p>
  Once inside the Admin Panel, we'll add new roles by going <ins>Agents -> Roles -> Add New Role</ins>.<br>
</p>
<p>
  
  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/cba9a2e8-3a27-4a81-a5d2-176efd7158fa)

</p>
<p>
  Here we can create any role we want with any permission we need it to have, for example: We need a role that has the same power as an Admin and can do any changes as needed, we'll call it **SuperAdmin**.<br>
  As said before, we want this role to have as many permissions as possible, so we'll check all the boxes we can and then add the role.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/93f4b6fb-d9f0-4a9a-944e-2f85f92bd738)

</p>
<p>
  As you can see, our new Role has been added, and we'll now be able to assign it to an agent soon.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/5d5b5aee-e7bb-432f-8763-aa0ac802d26e)

</p><br/>
<h2>Departments</h2>
<p>Departments are close to roles in that they help keep things organized. We can use and configure departments so that any agent inside it can fulfill the corresponding issue the department was made for without caring for the agent's role.<br>
By going <ins>Agents -> Departments -> Add New Department</ins> we can create a new department.</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/48ed7373-6e0f-47b6-ae57-c6f194bed4d3)

</p>
<p>
  For this example we'll create a department named **System Admins**, in the creation window we can see a lot of configurable options, like the type of department, ticket assignment and SLA that help define what a Department's Specialty is. For this, we'll just let all in default, as this is just and example.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/7de6d8af-ee56-41bf-bbd1-c7a1909d3803)
![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/a744781f-2ce7-4986-abb1-57c79725acad)

</p>
<br/>
<h2>Teams</h2>
<p>
  Teams are a versatile form of grouping that let you pull agents from different departments into a single group to solve a very specific problem. Are very helpful when you need a group of very specific people (like the best technician of every department, etc.).<br>
  To create a new team, go to <ins>Agents -> Teams -> Add New team</ins>.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/f0dfa81f-72cb-4fac-9e8a-0352b3241d2f)

</p>
<p>
  You can create a with the name of the specific topic that needs attention and add the members now or later. Once you create the team, it stays in the team tab until deleted. As you can see, we added another team named "Level II Support".
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/2fde8809-129b-4d4c-9e42-da524f0ced6f)
![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/d2df3c18-db25-4b08-ac58-1bee65fd0723)

</p><br/>
<h2>Tickets</h2>
<p>
  Ticket refers to a user issuing a complaint or problem to the system in order for it to be assigned the proper department, urgency and solution as soon as possible.<br>
  We'll now configure osTicket to allow anyone to send tickets. By going to <ins>Admin Panel -> Settings -> User Settings</ins> and once here we can decide if we want to allow anyone or just registered users to send tickets by leaving or checking the shown below option. For this example, we'll leave it unchecked to allow anonymous ticket submission.
</p>
<p>

   ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/c525e151-4d46-44ff-b10b-dca8903719d1)

</p>
<br/>
<h2>Agents</h2>
<p>Agents are the ones in charge of solving the tickets that come to the help desk. Each agent can be assigned roles, departments and teams.<br>
  To create a new agent, we go to <ins>Admin Panel -> Agents -> Add New Agent</ins>.
</p>
<p>

 ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/6f29689e-3697-4bde-ace1-7d8076e7ffc7)
 
</p>
<p>
  While creating a new agent, you must assign a username and a password that can be later changed by the agent. You can also assign departments and roles, or even add to a team. In this example, we'll create an agent with administrator capabilities that belongs in the "System Administrator" department and has the "SuperAdmin" Role.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/a5cf1b93-3922-4a34-ba5b-b30123e898f8)
  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/9a4ef3f2-7e7d-4f6e-bc38-efc5442d7727)

</p>
<p>
  As you can see, the new agent appears now in the agent tab with all his relevant info.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/c8d42e2a-5918-40cd-8e27-d653da687f29)

</p>
<br/>
<h2>Users (Customers)</h2>
<p>
  User refers to a non-agent person that submits tickets. They can be registered or anonymous. In this example, let's create a new user by going to <ins>Agent Panel -> Users -> Add New User</ins>.
</p>
<p>
  
  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/bc86582d-1353-48ff-af14-3dc7159d79df)

</p>
<p>
  In this tab you can enter a name and an email in order to create a new user, and it will now appear inside the "User Directory".
</p>
<p>
  
  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/11b6b20d-6717-49f1-a289-0defb4642a10)

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/833d5bf7-2ed1-467a-885d-3cc56b11690d)

</p><br/>
<h2>SLA</h2>
<p>
  SLA or "Service Level Agreements" are a guarantee to the customer that their problem will be solved within a frame of time, depending on the urgency of the issue. You can stipulate an arrangement of SLA's for different reasons. For this example, we'll create 3 different ones:
  <ul>
    <li>SEV-A (1 Hour, 24/7)</li>
    <li>SEV-B (4 Hours, 24/7)</li>
    <li>SEV-C (8 Hours, within business hours)</li>
  <ul/><br>
  We can make a new SLA by going to <ins>Admin Panel -> Manage -> SLA</ins> and clicking "Add New SLA Plan".
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/cdbf1a98-96a6-490f-b1e4-f6e69a5945d8)

</p>
<p>
  While adding a new SLA, you must select a Name, a grace period for the problem to be solved and a schedule for the days it can be solved. You can see in the example below how it looks to create a new SLA and the screen after we created 3 of them.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/5febaa8a-532b-48f2-87d4-16ef5fb2da16)
![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/64a5074f-047a-4c78-a678-c2089b94f386)

</p><br/>
<h2>Help Topics</h2>
<p>
  Help Topics help pinpoint/categorize more easily the problem for the customer at the moment they create the ticket. For example, a customer may have a problem with their hardware and so, they submit their ticket to the help topic "Equipment Malfunction".<br>
  To create help topics, go to <ins>Admin Panel -> Manage -> Help Topics</ins> and click "Add New Help Topic".
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/afbedf6b-203a-4bd9-98e4-4c6360b535ac)

</p>
<p>
  Give your topic a name, status, type and parent if it applies as a subcategory of another already created help topic (ex. New Equipment Opinions -> General Feedback). Assign department, priority and SLA plan in the "New ticket options" tab.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/ab85c298-975c-441b-b3ad-7e22ed423c3a)
  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/6558f12e-5125-47f1-bb6c-52f05e7c28f8)


</p>
<p>
  After adding the new topic, you can see it appears along the other topics on the main tab.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/1ca10d09-75a8-4862-afe6-5bb0aadf57c8)

</p>
<br/>
<p>

[Part 3: Ticket Life Cycle](https://github.com/DsosaH/osticket-lifecycle)
  
</p>
