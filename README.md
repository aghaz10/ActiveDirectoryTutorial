<h1>SIEM Build with Azure VM & Sentinel (LIVE ATTACK Monitoring)-Home Lab</h1>

<h2>Description</h2>
In this project, I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. I observe live attacks (RDP Brute Force) from all around the world. I use a custom PowerShell script to look up the attackers' Geolocation information and plot it on the Azure Sentinel Map!
<br />
<br />
<img src="https://i.imghippo.com/files/nt6Nx1723132563.png" height="80%" width="80%"/>

<br />

<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>AzureVM</b>
- <b>AzureSentinel</b>
- <b>AzureLogAnalytics</b>

<h2>Environments Used </h2>

- <b>Windows 10 (VM on RDP)</b> (21H2)
- <b>MacOS Sonoma 14.5</b> (M1)

<h2>Build walk-through:</h2>

<p align="center">
Create VM: <br/>
<img src="https://i.imghippo.com/files/xFkBM1723132746.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>
Allow All in Firewall:  <br/><br/>
<img src="https://i.imghippo.com/files/rZ5w01723132962.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br/>
Create Log Analytics Workspace: <br/><br/>
<img src="https://i.imghippo.com/files/tUTFp1723133143.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
<br />
Connect Log Analtics to VM:  <br/><br/>
<img src="https://i.imghippo.com/files/IRznF1723133493.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
<br />
Set Up Azure Sentinel:  <br/><br/>
<img src="https://i.imghippo.com/files/xDfhG1723133623.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
<br />
Log into VM with RDP. Turn off Windows Firewall on VM  <br/>
<img src="https://i.imghippo.com/files/X4kNe1723133799.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
<br />
Get Geolocation.io API key. Run PowerShell Script to get GeoData from Attackers:  <br/><br/>
<img src="https://i.imghippo.com/files/N5fMv1723133938.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
<br />
Create custom log in LAW to sync custom log with custom/extract fields from custom log data:  <br/><br/>
<img src="https://i.imghippo.com/files/mW1Xg1723134110.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
<br />
Set Up Map in Sentinel based on Country. Observe live attacks plotted on map, including Attack Count!  <br/><br/>
<img src="https://i.imghippo.com/files/r1Y551723134288.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
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
