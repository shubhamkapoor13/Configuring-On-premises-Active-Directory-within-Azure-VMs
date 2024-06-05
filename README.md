# Configuring-On-premises-Active-Directory-within-Azure-VMs

<p align="center">
<img src="https://i.Imgur.com/tBg2A87.png" alt="Microsoft Active Directory Logo"/>
</p>

<h2>Active Directory Deployed in the Cloud (Microsoft Azure)</h2>
  
<p>In the last tutorial I installed Active directory within Azure Virtual Machines. This tutorial I will go through configuration of Active Directory.</p>

- Create an Admin User account, Organizational Unit, and New Employee to the Domain Admins Security Group. 
- Join the Client to the DC
- Set up Remote Desktop for users/non-administrative users.
- Create a Bunch of Users

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)
  
 <h2> Create an Admin User account and Organizational Units </h2>
 <p>Open Active Directory Users and Computers > Right click on mydomain.com > Click New > Click Organizational unit and create one for both: </p>
 
- _EMPLOYEES(NOTE: to make sure to put underscore and all words are in capital for powershell script)
- _ADMINS

<img src="https://i.imgur.com/b5p8ppc.png">
<img src="https://i.imgur.com/LSUMMZg.png">

Right Click on mydomain.com > Click to Refresh

 <h2>Create an Admin User Account</h2>
 <a>Right click on _ADMINS > Click New > Click User</a>
 
 <img src="https://i.imgur.com/ndS71kC.png">
 
 <b> Fill in Information and Create a Password</b>
 
 Uncheck: user must change password at next logon
 
 Check: Password never expires 
 
 <img src="https://i.imgur.com/Eq1OV2X.png">
 <img src="https://i.imgur.com/f0tESfY.png">
 
