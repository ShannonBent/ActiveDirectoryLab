<h1>Creating & Managing Active Directory Objects</h1>


<h2>Description</h2>
Project consists of creating and managing Active Directory objects involving the use of Active Directory Users and Computers tool to create user accounts, groups, and computer accounts, and to modify their attributes. This includes adding users to groups, setting up organizational units, and delegating administrative tasks. Establishing a Remote Desktop Connection requires enabling Remote Desktop on the target machine and using the RDC client to connect by entering the remote machine’s name and the necessary user credentials. These processes are essential for effective network and system administration.
<br />


<h2>Tools used</h2>

- <b>Active Directory Users and Computers</b> 
- <b>Remote Desktop Connection</b>

<h2>Environments Used </h2>

- <b>Windows Server</b>
- <b>Windows Client</b>

<h2>Lab walk-through:</h2>

<p align="center">
(Windows Server) <br/>
In the Active Directory Users and Computers, navigate to the cyber.local domain and create a new OU named "Sales" <br/>
<img src="https://i.imgur.com/Ahi53J4.png) width="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Within the cyber.local domain Sales OU, create a new user named "Salesperson1" with a set password. Uncheck the "user must change password at next logon" box  <br/>
<img src="https://i.imgur.com/TDfTo3D.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/S9sfiWA.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Within the cyber.local domain Sales OU, create a new group named "Sales-GRP" <br/>
<img src="https://i.imgur.com/kD2zfZt.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Within the cyber.local domain Sales OU, add the user "Salesperson1" to the "Sales-GRP" group <br/>
<img src="https://i.imgur.com/3VNGhVd.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Within the cyber.local domain Sales OU, create a new user named "Sales-Template" with a set password. Uncheck the "user must change password at next logon" box <br/>
<img src="https://i.imgur.com/ZoMjOAJ.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/20D5rdd.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Within the cyber.local domain Sales OU, configure the "Sales-Template" user with these settings: Department: Sales, Company: cyber.local; Deny logon on Sundays; Add "Sales-Template user to the "Sales-GRP" group <br/>
<img src="https://i.imgur.com/KwIowDF.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/YbPyaMm.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/9zsQwtR.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Add the "Salesperson1" user to the "Domains Admins" group  <br/>
<img src="https://i.imgur.com/fVvp9Pm.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
(Windows Client) <br/>
Switch over to the Windows Client tab and establish a remote connection using the "Remote Desktop Connection". In the computer field, type in Windows_Client and click connect <br />
<img src="https://i.imgur.com/kRDVcAW.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Authenticate with the users credentials and a remote connection has been established <br/>
<img src="https://i.imgur.com/oDxBcmL.png) width="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ayql8uD.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
