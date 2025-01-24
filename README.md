<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Deploying Active Directory in the Cloud (Azure)</h1>
This tutorial outlines the deployment of active directory within Azure Virtual Machines.<br />
Prerequisites-

- have a domain controller running on a virtual machine

- have a client side pc running on a virtual machine 


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)
<h2>High-Level Deployment and Configuration Steps</h2>
Today we will be deploying and configuring active directory using azure vms

- Install active direcotry domain services onto the domain controller and setup a new forest (mydomain.com)
- Create orginization units for your users
- Create a domain admin user and normal user within active directory users and computers
- Join client 1 to the domain (mydomain.com) using your newly created admin profile
- log into doamin controller as the admin profile you created and verify client 1 is joined to the dc

<h2>Deployment Step 1</h2>

![Screenshot 2025-01-24 121826](https://github.com/user-attachments/assets/2160721c-1623-43ae-b8b8-85832276dd74)


</p>
<p>
Login into your domain controller and install active directory services, set up a new forest (mydomain.com)
</p>
<br />

<p>

  ![Screenshot 2025-01-24 122230](https://github.com/user-attachments/assets/42983e5a-c730-41f8-89bf-0e97ec576902)

</p>
<p>

  Create oginizational units within active directory-users and computers
 
  Create a domain admin and a normal user

  Restart DC1 and Client1
Log back into your vm's using the admin profile you created
</p>
<br />

<p>

  ![Screenshot 2025-01-24 122521](https://github.com/user-attachments/assets/56c8946a-6a9c-4188-94f8-bfc3337c0a74)

</p>
<p>
Logged into client 1 as your admin account

  Go into your system preferences
  
  Join client 1 to your domain (mydomain.com)
</p>
<br />

![Screenshot 2025-01-24 122801](https://github.com/user-attachments/assets/d2d1d5bb-8f00-46dd-8a69-6054b0b6bfbf)

Log back into the DC as your admin account. 

Observe active directory and confirm that client 1 has joined the domain.

