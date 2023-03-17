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
- Command Prompt

<h2>Operating Systems Used </h2>

- Windows Server 2022

<h2>High-Level Steps</h2>

- Step 1: Login remotely to Windows Server
- Step 2: Open Group Policy Management in Server Manager
- Step 3: Enable Group Policies
- Step 4: Review Changes in Command Prompt

<h2>Actions and Observations</h2>

<h2>Login Remotely to Windows Server</h2>
<p>
<img src="https://imgur.com/bgRhNG6.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
Assuming that we have already created a virtual machine running on Windows Server and logged in to remote desktop, open Server Manager on the virtual machine. Click on "Tools" and "Group Policy Management." This role houses various policies that manage both Windows and User configurations.
</p>
<br />
<h2>Create a Group Policy Object (GPO)</h2>
<p>
<img src="https://imgur.com/Y1pNm05.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, right-click on your "Created Domain" and select "Create a GPO". Next, you can name the file to anything that you prefer. For this demostration, we will name it "Custom Setting". GPO is a file to configure users and how to use their computer.
</p>
<br />
<h2>Edit Group Policy Object (GPO)</h2>
<p>
<img src="https://imgur.com/fYTqfGc.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
After creating the GPO, we can begin to edit the various features for both computers and user. Right-click on the GPO that was previously created and click on "Edit". Next, you will see in the righ hand corner for "Computer Configuration" and "User Configuration". Under each, we can see that they are policy and preference folders that system administrators can use to customize computer or user settings.
</p>
<br />
<h2>Edit Computer Configuration Password Policy</h2>
<p>
<img src="https://imgur.com/KL9FKD3.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this demonstration, we can toggle under "Computer Configuration" to "Policies" --> "Windows Settings" --> "Security Settings" --> "Account Settings" --> "Password Policy".
</p>
<br />
<h2>Edit Computer Configuration Password Policy Continued</h2>
<p>
<img src="https://imgur.com/BliPLK1.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
Under Password policies for computer configuration, it has various polices that can be created such as length, age, or complexity of a password. In this example, we can edit the length of characters for a password by setting the password to have a minimum of 8 characters.
</p>
<br />
<h2>Edit User Configuration Desktop Policy Continued</h2>
<p>
<img src="https://imgur.com/IhQcHCr.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
Under Desktop policies under User Configuration, we can control the features that are added to the user's desktop. For instance, we can make the decision to Remove the Recycle Bin item from the user's desktop. Group Policy allows the system administrator control various features for computers and users, based on the requirements of the company.
</p>
<br />
<h2>Review Group Policy Changes in Command Prompt</h2>
<p>
<img src="https://imgur.com/h8eFzcS.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
Under Command Prompt, we can review the changes that were made in Group Policy. Open Command Prompt as and administrator --> Enter "gpresult /r". This can be super helpful in notcing the changes that were previously made by the admin team.
</p>
<br />
