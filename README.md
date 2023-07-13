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
Create Ubuntu Server as attack VM: <br/>
<img src="EDR-Home-Lab/1- Create Ubuntu Server as attack VM.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Create Windows 10 VM as the vulnerable computer:  <br/>
<img src="EDR-Home-Lab/2- Create Windows 10 VM as Vulnerable VM.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Install LimaCharlie on Windows 10 VM for Endpoint, Detection, and Response: <br/>
<img src="EDR-Home-Lab/3-Install Lima Charlie for EDR.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Configure sensor in LimaCharlie to generate logs:  <br/>
<img src="EDR-Home-Lab/4 Installing LC Sensor on Windows VM.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Create a rule in LimaCharlie to ingest Sysmon logs:  <br/>
<img src="EDR-Home-Lab/5-Create Rule to Collect SysMon Logs.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Access Ubuntu Server through SSH using Powershell:  <br/>
<img src="EDR-Home-Lab/6 Access linux vm using ssh thorugh powershell.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Download Sliver on Ubuntu Server:  <br/>
<img src="EDR-Home-Lab/7- Download Sliver on Linux VM.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Use Sliver to generate malicious payload:  <br/>
<img src="EDR-Home-Lab/8- Create Malware payload in sliver.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Verify Malware is working:  <br/>
<img src="EDR-Home-Lab/9-Verify Malware is working.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Begin attack by collecting information on infected machine:  <br/>
<img src="EDR-Home-Lab/10-Gather into on infected vm.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Examine network traffic using Netstat: <br/>
<img src="EDR-Home-Lab/11- Examine network traffic with netstat.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Review logs created in EDR:  <br/>
<img src="EDR-Home-Lab/12- Examine EDR logs.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
View file hash for the malicious download: <br/>
<img src="EDR-Home-Lab/13-run-file-hash-for-malicious-downlaod-through-virus-total.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Search for the file hash in VirusTotal:  <br/>
<img src="EDR-Home-Lab/14-run-file-hash-for-malicious-downlaod-through-virus-total.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Preform an LSASS Credential Dump:  <br/>
<img src="EDR-Home-Lab/15-preform-LSASS-dump.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Review logs created by preforming LSASS dump:  <br/>
<img src="EDR-Home-Lab/16 Detect-LSASS-Dump.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Create a rule to report LSASS credential dumping:  <br/>
<img src="EDR-Home-Lab/17-Create-rule-to-report-LSASS-dump.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Verify the new rule is functioning as designed:  <br/>
<img src="EDR-Home-Lab/18-Verify-new-rule-took-effect.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Attempt Volume Shadow Copies Deletion:  <br/>
<img src="EDR-Home-Lab/19-Attempt-Volume-Shadow-Copies-Deletion.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Review logs created by VSS deletion attempt:  <br/>
<img src="EDR-Home-Lab/20-Detect-VSC-Deletion-Attempt.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Create a rule to detect and block a VSS deletion attempt:  <br/>
<img src="EDR-Home-Lab/21-Create-Rule-To-Block-VSS-Attack.png" height="80%" width="80%" alt="AD Lab Steps"/>
<br />
<br />
Verify the new rule terminates our connection to the infected machine:  <br/>
<img src="EDR-Home-Lab/22-Verify-Rule.png" height="80%" width="80%" alt="AD Lab Steps"/>
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
