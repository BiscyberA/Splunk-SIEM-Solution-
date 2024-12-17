<h1>Splunk(SIEM Solution) Home Lab</h1>
- [Collected,Ingested and Analyzed VPNlogs]

<h2>Description</h2>
In this lab we will cover basics of Splunk, the leading SIEM solution for collecting,Analyzing and Correlating logs from various log sources in real-time.We will install,navigate and go through the various components of splunk and its functionality, and then ingest logs into splunk instance and try to practice some commands on the logs. 
<br />

<h2>Tool Used</h2>

- <b>Splunk Enterprise</b> 

<h2>Environments Used </h2>

- <b>Web Access Logs</b>
- <b>Ubuntu </b> 

<h2>Lab walk-through:</h2>

<p align="center">
I installed splunk on Ubuntu and this is the home apge after the installation <br/>
<img src="https://i.postimg.cc/gjq5s3qH/Screenshot-2024-12-16-131840.png"/>
<br />
<br />
I navigated to the paage where I can add sample logs to splunk by clicking on upload <br/>
<img src="https://i.postimg.cc/SxNsWr7V/Screenshot-2024-12-16-132222.png" />
<br />
<br />
I uploaded the sample log and clicked next<br/>
<img src="https://i.postimg.cc/dtJtYBXv/Screenshot-2024-12-16-140346.png" />
<br />
<br />
Here is the preview of the sample log and then clicked next<br/>
<img src="https://i.postimg.cc/T3wdyPf4/Screenshot-2024-12-16-140522.png" />
<br />
<br />
I ckicked on create index to create a new index<br/>
<img src="" />
<br />
<br />
Index field filled out and saved  <br/>
<img src="" />
<br />
<br />
Navigating Splunk: Splunk bar includes: Messages(For system level messages),Settings(For configuration),Activity(To review job progress),Help and
Find(For Search)<br/>
<img src="https://imgur.com/h7u1VT1.png" height="80%" width="80%" />
<br />
<br />
App Panel: Allows for ability to see installed apps on splunk instance with one of its default App:Search and Reporting<br/>
<img src="https://imgur.com/IKo5OkY.png" height="80%" width="80%" />
<br />
<br />
Explore Splunk: Gives quick links to add data,add new apps and access splunk documentation.<br/>
<img src="https://imgur.com/1e10xFB.png" height="80%" width="80%" />
<br />
<br />
Splunk Dashboard: No Dashboard are display by default: You an create Dashboard<br/>
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
There are few ways we send data to splunk such as Monitor, forwarder but we will use the upload option: A page like this will appear <br/>
<img src="https://imgur.com/jJb4mk4.png" height="80%" width="80%" />
<br />
<br />
This page allows you to select the Log Source(VPNlogs) stored on our computer:Select the file from your Computer, upload and Click Next<br/>
<img src="https://imgur.com/jJb4mk4.png" height="80%" width="80%" />
<br />
<br />
Select Source Type :This page shows how splunk sees my log source type.:Splunk identified it as json. Click Next<br/>
<img src="https://imgur.com/0FMAyuK.png" height="80%" width="80%" />
<br />
<br />
Create an Index where the logs will be dumped:Index takes the data uploaded and normalizes it into value pairs, data type and store as events.Click save<br/>
<img src="https://imgur.com/T51Oaea.png" height="80%" width="80%" />
<br />
<br />
Create a host field value with a name from which the events originated from.In this event is from VPN connection: Select the index created in the dropdown and Click review <br/>
<img src="https://imgur.com/tLFU5RS.png" height="80%" width="80%" />
<br />
<br />
Review Page shows the Input Type, File Name, Source Type and the created Host and Index.Click Submit and then Click Start Searching<br/>
<img src="https://imgur.com/EVkwzdm.png" height="80%" width="80%" />
<br />
<br />
Page Appears showing all the logs been ingested and  indexed(with field-values and data types) into Splunk Instance <br/>
<img src="https://imgur.com/nlhqrf9.png" height="80%" width="80%" />
<br />
<br />
 Below shows number of events indexed and ingested into the splunk instnace: 5724 Events<br/>
<img src="https://imgur.com/LXqZ2eW.png" height="80%" width="80%" />
<br />
<br />
I index search on the Username Maleena to identify how many Log Events was captured: 120 Events <br/>
<img src="https://imgur.com/khrQpZH.png" height="80%" width="80%" />
<br />
<br />
I index search the Username associated with the IP Address 107.14.182.38: Smith has the IP <br/>
<img src="https://imgur.com/JasJVty.png" height="80%" width="80%" />
<br />
<br />
I index search the number of events originated from all countries except France: I index search France event and subtract it from total event. <br/>
<img src="https://imgur.com/0W69cOX.png" height="80%" width="80%" />
<br />
<br />

<h2>Conclusion</h2>
Again, this is just a basic overview of Splunk where I just uploaded a network centric data(VPN LOGS) into Splunk Instance and did a simple index searches.We can also have a Splunk forwader which is one of the component of Splunk install and configured on Host machine to capture host centric logs example(winEvent logs) and forwards it to the Splunk instance for investigation or Analysis(This is going to be my next project). We can also create table for specific Indexes or field value types to reduce search.




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
