<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Azure Active Directory"/>
</p>

<h1>Group Policy Management</h1>
In this tutorial, we observe Group Policy Management in Server Manager and explore a couple of features. Group Policy allows the system adminstrator to configure policies to manage users and their envrionments. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Server Manager
- Group Policy Management

<h2>Operating Systems Used </h2>

- Windows Server 2022

<h2>High-Level Steps</h2>

- Step 1: Login remotely to Windows Server
- Step 2: Open Group Policy Management in Server Manager
- Step 3: Enable Group Policies

<h2>Actions and Observations</h2>

<h2>Login Remotely to Windows Server</h2>
<p>
<img src="https://imgur.com/bgRhNG6.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Assuming that we have already created a virtual machine running on Windows Server and logged in to remote desktop, open Server Manager on the virtual machine. Click on "Tools" and "Group Policy Management." This role houses various policies that manage both Windows and User configurations.
</p>
<br />
<h2>Create a Group Policy Object (GPO)</h2>
<p>
<img src="https://imgur.com/Y1pNm05.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, right-click on your "Created Domain" and select "Create a GPO". Next, you can name the file to anything that you prefer. For this demostration, we will name it "Custom Setting". GPO is a file to configure users and how to use their computer.
</p>
<br />
<h2>Edit Group Policy Object (GPO)</h2>
<p>
<img src="https://imgur.com/fYTqfGc.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
After creating the GPO, we can begin to edit the various features for both computers and user. Right-click on the GPO that was previously created and click on "Edit". Next, you will see in the righ hand corner for "Computer Configuration" and "User Configuration". Under each, we can see that they are policy and preference folders that system administrators can use to customize computer or user settings.
</p>
<br />
<h2>Edit Computer Configuration Policy</h2>
<p>
<img src="https://imgur.com/KL9FKD3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this demonstration, we can toggle under "Computer Configuration" to "Policies" --> "Windows Settings" --> "Security Settings" --> "Account Settings" --> "Password Policy".
</p>
<br />
