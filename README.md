<h1>Splunk(SIEM Solution) Home Lab</h1>
- [Collecting,Ingesting and Analyzing VPNlogs]

<h2>Description</h2>
In this lab we will cover basics of Splunk, the leading SIEM solution for collecting,Analyzing and Correlating machines and network logs in real-time.We will install,navigate and go through the various components of splunk and its functionality, and then ingest vpnlogs into splunk instance and try to analyze the logs. 
<br />

<h2>Tool Used</h2>

- <b>Splunk Enterprise</b> 

<h2>Environments Used </h2>

- <b>VPN Logs</b>
- <b>Windows 11</b> (21H2)

<h2>Lab walk-through:</h2>

<p align="center">
Installing Splunk Enterprise on Windows 11 Host: Check the box to accept License Agreement and Click Next<br/>
<img src="https://imgur.com/lhxJcE0.png" height="80%" width="80%"/>
<br />
<br />
Create an Admin Account and Click Next<br/>
<img src="https://imgur.com/wCXTRQC.png" height="80%" width="80%" />
<br />
<br />
Click install<br/>
<img src="https://imgur.com/w280tvX.png" height="80%" width="80%" />
<br />
<br />
Setup Installing<br/>
<img src="https://imgur.com/wu3MgE5.png" height="80%" width="80%" />
<br />
<br />
Installation Complete: Click finish<br/>
<img src="https://imgur.com/NO49ZCC.png" height="80%" width="80%" />
<br />
<br />
Splunk Enterprise is launch with the default home page <br/>
<img src="https://imgur.com/EflRwzk.png" height="80%" width="80%" />
<br />
<br />
Navigating Splunk: Splunk bar includes: Messages(For system level messages),Settings(For configuration),Activity(To review job progress),Help and
Find<br/>
<img src="https://imgur.com/h7u1VT1.png" height="80%" width="80%" />
<br />
<br />
App Panel: Allows for ability to see installed apps on splunk instance<br/>
<img src="https://imgur.com/IKo5OkY.png" height="80%" width="80%" />
<br />
<br />
Explore Splunk: Gives quick links to add data,add new apps and access splunk documentation.<br/>
<img src="https://imgur.com/1e10xFB.png" height="80%" width="80%" />
<br />
<br />
Splunk Dashboard: No Dashboard are display by default.<br/>
<img src="https://imgur.com/6DNwyhi.png" height="80%" width="80%" />
<br />
<br />
Splunk Dashboard Continues: You can choose from a range of dashboard from the dropdown menu or by visiting the Dashboard listing page<br/>
<img src="https://imgur.com/vrodWdX.png" height="80%" width="80%" />
<br />
<br />
Adding or Ingesting Data into Splunk Instance: Click on Add data on the Explore Splunk home page and a new page like this appears<br/>
<img src="https://imgur.com/XPF50bQ.png" height="80%" width="80%" />
<br />
<br />
Use upload option: A page like this will appear <br/>
<img src="https://imgur.com/jJb4mk4.png" height="80%" width="80%" />
<br />
<br />
Log Source: Select the file from your Computer: Click Next<br/>
<img src="https://imgur.com/jJb4mk4.png" height="80%" width="80%" />
<br />
<br />
Select Source Type : json selected : Click Next<br/>
<img src="https://imgur.com/0FMAyuK.png" height="80%" width="80%" />
<br />
<br />
Create an Index where the logs will be dumped: Click save<br/>
<img src="https://imgur.com/T51Oaea.png" height="80%" width="80%" />
<br />
<br />
Create a hostname associated with the logs: Select the index in the dropdown and Click review <br/>
<img src="https://imgur.com/tLFU5RS.png" height="80%" width="80%" />
<br />
<br />
Review Page: Click Submit and then Click Start Searching<br/>
<img src="https://imgur.com/EVkwzdm.png" height="80%" width="80%" />
<br />
<br />
Page Appears showing all the logs been ingested and  indexed into Splunk Instance <br/>
<img src="https://imgur.com/ZAYo7gj.png" height="80%" width="80%" />
<br />
<br />

Watch the Video Tutorial for further Analysis of the Logs<br/>

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
