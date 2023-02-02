<h1>Splunk(SIEM Solution) Home Lab</h1>
- [Collecting,Ingesting and Analyzing VPNlogs]

<h2>Description</h2>
In this lab we will cover basics of Splunk, the leading SIEM solution for collecting,Analyzing and Correlating machines and network logs in real-time.We will install,go through the various components of splunk and its functionality, and then ingest vpnlogs into splunk instance and try to analyze the logs. 
<br />

<h2>Tool Used</h2>

- <b>Splunk Enterprise</b> 

<h2>Environments Used </h2>

- <b>VPN Logs</b>
- <b>Windows 11</b> (21H2)

<h2>Lab walk-through:</h2>

<p align="center">
Installing Splunk Enterprise on Windows 11 Host: Check to accept License Agreement and Click Next<br/>
<img src="https://imgur.com/9De1u6V.png" height="80%" width="80%"/>
<br />
<br />
Create an Admin Account and Click Next<br/>
<img src="https://imgur.com/PfJWmAY.png" height="80%" width="80%" />
<br />
<br />
Click install<br/>
<img src="https://imgur.com/ffEAy1E.png" height="80%" width="80%" />
<br />
<br />
Setup Installing<br/>
<img src="https://imgur.com/pTFg5As.png" height="80%" width="80%" />
<br />
<br />
Installing Complete: Click finish<br/>
<img src="https://imgur.com/ZzimULX.png" height="80%" width="80%" />
<br />
<br />
Splunk Enterprise is launch with a default home page <br/>
<img src="https://imgur.com/IMCTsBC.png" height="80%" width="80%" />
<br />
<br />
Clicked on Basic Network Scan: Opens a new scan page: Input name of scan: Input target Ip address(Windows10 host):Saved scan<br/>
<img src="https://imgur.com/YImsxPd.png" height="80%" width="80%" />
<br />
<br />
Launched Scan : Scan Running <br/>
<img src="https://imgur.com/VGNr6JT.png" height="80%" width="80%" />
<br />
<br />
Scan Completed: Showing Scan Details :Color Coding severity of Vulnerability:<br/>
<img src="https://imgur.com/zqYgTGP.png" height="80%" width="80%" />
<br />
<br />
Vulnerabilities Results:  <br/>
<img src="https://imgur.com/xY9htKp.png" height="80%" width="80%" />
<br />
<br />
SMB Vulnerability:  <br/>
<img src="https://imgur.com/qFQYWWy.png" height="80%" width="80%" />
<br />
<br />
Enabled Remote Registry:  <br/>
<img src="https://imgur.com/fey5FJi.png" height="80%" width="80%" />
<br />
<br />
Change User Account Control Settings to "Never Notify:  <br/>
<img src="https://imgur.com/v6snDMP.png" height="80%" width="80%" />
<br />
<br />
Enabled Files and Printer Sharing:  <br/>
<img src="https://imgur.com/fjhQ4FG.png" height="80%" width="80%" />
<br />
<br />
Added LocalAccountTokenFilterPolicy to Registry:  <br/>
<img src="https://imgur.com/xO2A7oo.png" height="80%" width="80%" />
<br />
<br />
Set LocalAccountTokenFilterPolicy value to 1:  <br/>
<img src="https://imgur.com/FhOBlXf.png" height="80%" width="80%" />
<br />
<br />
Reconfigured my scan to perform a credential scan:  <br/>
<img src="https://imgur.com/GxsX0Ze.png" height="80%" width="80%" />
<br />
<br />
Input the credential and saved the scan:  <br/>
<img src="https://imgur.com/bDhNch5.png" height="80%" width="80%" />
<br />
<br />
Credential Scan Completed: Showing Scan Details :Color Coding severity of Vulnerability:  <br/>
<img src="https://imgur.com/GeYZKuW.png" height="80%" width="80%" />
<br />
<br />
Credential Scan Vulnerabilities Results :  <br/>
<img src="https://imgur.com/wrSyBdB.png" height="80%" width="80%" />
<br />
<br />
Mixed Result Details:Mixture of critical,High,and Info <br/>
<img src="https://imgur.com/2XQxNc9.png" height="80%" width="80%" />
<br />
<br />
Input the credential and saved the scan:  <br/>
<img src="https://imgur.com/bDhNch5.png" height="80%" width="80%" />
<br />
<br />
Input the credential and saved the scan:  <br/>
<img src="https://imgur.com/bDhNch5.png" height="80%" width="80%" />
<br />
<br />
Input the credential and saved the scan:  <br/>
<img src="https://imgur.com/bDhNch5.png" height="80%" width="80%" />
<br />
<br />
Input the credential and saved the scan:  <br/>
<img src="https://imgur.com/bDhNch5.png" height="80%" width="80%" />






Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
