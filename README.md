<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Setup Domain Controller in Azure
- Set Domain controller's NIC private IP address to be static
- Disable windows firewall in the VM for testing connectivity
- Create client-1 or another VM in azure
- Set client-1's DNS setting to DC-1's private IP address

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/B7wwr2O.png">
</p>
<p>
To set up active directory first you'll need to create a domain controller virtual machine thats sorts of act like the back end access to the other virtual machine you'll end up creating.
</p>
<br />

<p>
<img src="https://i.imgur.com/Z1GaDME.png">
</p>
<p>
For the last step in setting up active directory you'll need your Domain controllers NIC private IP address to be static meaning it doesn't change.
</p>
<br />

<p>
<img src="https://i.imgur.com/jWHzAjr.png">
</p>
<p>
Disabling windows firewall allows for testing connectivity within the virtual machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/1Bcztb3.png">
</p>
<p>
For active directory to be fully functional you'll need another virtual machine which will basically hold the users you'll create and its sort of like the computer they can use if you assign them permissions to it.
</p>
<br />

<p>
<img src="https://i.imgur.com/Y7etExm.png">
</p>
<p>
For connectivity and for active directory this is the most crucial step because its basically what connects the two computer together.
</p>
<br />
