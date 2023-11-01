<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-installation Configuration</h1>
This is the next part of the tutorial, where we'll configure osTicket so it is functional.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
<h2>Configuring Roles</h2>
<p>
  osTicket, like most ticketing systems, depend on a hierarchy in order to correctly deliver the ticket depending on how urgent and dificult a task is. For this reason we need to create and assign the correct roles.<br>
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
  As said before, we want this role to have as much permissions as possible, so we'll check all the boxes we can and then add the role.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/93f4b6fb-d9f0-4a9a-944e-2f85f92bd738)

</p>
<p>
  As you can see, our new Role has been added and we'll now be able to assign it to an agent soon.
</p>
<p>

  ![image](https://github.com/DsosaH/osticket-postconfg/assets/148100125/5d5b5aee-e7bb-432f-8763-aa0ac802d26e)

</p><br/>
<h2>Departments</h2>
