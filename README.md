<h1>Endpoint Detection and Response Home Lab</h1>


<h2>Description</h2>
For this project, I created to Virtual machines to serve as my home lab. The first was a Linux VM, running Ubuntu Server. This was my attack platform. I used this machine to create noise and simulate attacks for my EDR LimaCharlie to detect. The second VM was a Windows 10 VM. This served as my vulnerable computer. I was able to execute malware on this VM through a program called Sliver through Powershell. This gave me administrative access to the Windows 10 VM.  
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>VMware Workstation</b>
- <b>Ubuntu Server</b>
- <b>Windows 10 Pro</b>

<h2>Program walk-through:</h2>

<p align="center">
Create Windows Server 2019 VM: <br/>
<img src="AD Home Lab/1 Create Server VM.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Configure Active Directory:  <br/>
<img src="AD Home Lab/2 Configure AD.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Add New User in AD Manually: <br/>
<img src="AD Home Lab/3 Add user in AD.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Connect Server to the Internet:  <br/>
<img src="AD Home Lab/4 Connect Server to the Internet.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Configure DHCP Server :  <br/>
<img src="AD Home Lab/5 Configure DHCP server.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Script for using Powershell to add 1000 users to AD:  <br/>
<img src="AD Home Lab/6 Script for creating 1k users.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Run Script in Powershell to create new users:  <br/>
<img src="AD Home Lab/7 Running script to create users.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Create Client VM using Windows 10:  <br/>
<img src="AD Home Lab/8 Create Client VM.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Final Set Up of Domain Controller:  <br/>
<img src="AD Home Lab/9 Final Set up of Domain Controller.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Users Added to AD:  <br/>
<img src="AD Home Lab/10 Users Added to AD.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Create Windows Server 2019 VM: <br/>
<img src="AD Home Lab/1 Create Server VM.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Configure Active Directory:  <br/>
<img src="AD Home Lab/2 Configure AD.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Add New User in AD Manually: <br/>
<img src="AD Home Lab/3 Add user in AD.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Connect Server to the Internet:  <br/>
<img src="AD Home Lab/4 Connect Server to the Internet.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Configure DHCP Server :  <br/>
<img src="AD Home Lab/5 Configure DHCP server.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Script for using Powershell to add 1000 users to AD:  <br/>
<img src="AD Home Lab/6 Script for creating 1k users.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Run Script in Powershell to create new users:  <br/>
<img src="AD Home Lab/7 Running script to create users.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Create Client VM using Windows 10:  <br/>
<img src="AD Home Lab/8 Create Client VM.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Final Set Up of Domain Controller:  <br/>
<img src="AD Home Lab/9 Final Set up of Domain Controller.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Users Added to AD:  <br/>
<img src="AD Home Lab/10 Users Added to AD.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Client Terminal Added in AD:  <br/>
<img src="AD Home Lab/11 Client Terminal Added in AD.png" height="80%" width="80%" alt="AD Lab Steps"/>
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
