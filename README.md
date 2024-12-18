<h1>Splunk(SIEM Solution) Home Lab</h1>
- [Ingested and Query Web Access Logs With Various SPL Commands]

<h2>Description</h2>
In this lab we will cover basics of Splunk, the leading SIEM solution for collecting,Analyzing and Correlating logs from various log sources in real-time.We will install,navigate and go through the various components of splunk and its functionality, and then ingest logs into splunk instance and practice some commands on the logs. 
<br />

<h2>Tools Used</h2>

- <b>Splunk Enterprise</b> 

<h2>Environments Used </h2>

- <b>Web Access Logs</b>
- <b>Ubuntu </b> 

<h2>Lab walk-through:</h2>

<p align="center">
I installed splunk on Ubuntu and this is the home page after the installation <br/>
<img src="https://i.postimg.cc/V5yg7m45/Screenshot-2024-12-16-131840.png"/>
<br />
<br />
I navigated to the page where I can add sample logs to splunk by clicking on upload <br/>
<img src="https://i.postimg.cc/13KxNj5D/Screenshot-2024-12-16-132222.png" />
<br />
<br />
I uploaded the sample log, I clicked next<br/>
<img src="https://i.postimg.cc/5ym5mLHK/Screenshot-2024-12-16-140546.png" />
<br />
<br />
Here is a preview of the sample log, I clicked next<br/>
<img src="https://i.postimg.cc/7h19QjRV/Screenshot-2024-12-16-140640.png" />
<br />
<br />
I ckicked on create index to create a new index<br/>
<img src="https://i.postimg.cc/qRs2kyGB/Screenshot-2024-12-16-140706.png" />
<br />
<br />
Index field filled out and saved  <br/>
<img src="https://i.postimg.cc/PJ6px4vH/Screenshot-2024-12-16-140822.png" />
<br />
<br />
Reviewed setup. I clicked submit to add data<br/>
<img src="https://i.postimg.cc/kMwtfn1H/Screenshot-2024-12-16-140853.png" />
<br />
<br />
Web access Log successfully uploaded<br/>
<img src="https://i.postimg.cc/W1qFN0NR/Screenshot-2024-12-16-140906.png" />
<br />
<br />
Queried the index to veiw ingested logs<br/>
<img src="https://i.postimg.cc/W35b64N6/Screenshot-2024-12-16-141057.png" />
<br />
<br />
Wrote a query to view http status code great than 200<br/>
<img src="https://i.postimg.cc/BvMGRwrJ/Screenshot-2024-12-16-150457.png" />
<br />
<br />
Wrote a query to view http status code great than or equal to 400<br/>
<img src="https://i.postimg.cc/Jz80Lv2X/Screenshot-2024-12-16-150627.png" />
<br />
<br />
Wrote a query to view http METHOD for GET or POST<br/>
<img src="https://i.postimg.cc/m2DVSpwQ/Screenshot-2024-12-16-151526.png" />
<br />
<br />
Wrote a query to view IPs that starts with 100<br/>
<img src="https://i.postimg.cc/MHG0dXyW/Screenshot-2024-12-16-152015.png" />
<br />
<br />
Wrote a query with the stats command to view a list of all the IPs in the logs<br/>
<img src="https://i.postimg.cc/fbL0G1VK/Screenshot-2024-12-16-214545.png" />
<br />
<br />
Wrote a query with the sort command to view a list of IPs with the top values in the logs<br/>
<img src="https://i.postimg.cc/Bnv6bHJZ/Screenshot-2024-12-16-214733.png" />
<br />
<br />
I used the head command to list the first 5 values<br/>
<img src="https://i.postimg.cc/0j8v31Q5/Screenshot-2024-12-16-214847.png" />
<br />
<br />
I used the table command to create a table for various fields<br/>
<img src="https://i.postimg.cc/4Nykh5H0/Screenshot-2024-12-16-215159.png" />
<br />
<br />
I used the dedup command to remove duplicate values of occurance<br/>
<img src="https://i.postimg.cc/Wp9xjkYw/Screenshot-2024-12-16-215645.png" />
<br />
<br />
I used the rename command to renamed the various column <br/>
<img src="https://i.postimg.cc/Hx6vpqzk/Screenshot-2024-12-16-220346.png" />
<br />
<br />
I used the timechart to view specific count of IP overtime<br/>
<img src="https://i.postimg.cc/Jz8F55sm/Screenshot-2024-12-16-221917.png" />
<br />
<br />
I used the search command to search event with strings Nmap<br/>
<img src="https://i.postimg.cc/LswBNmxf/Screenshot-2024-12-16-222444.png" />
<br />
<br />
I used the iplocation command to view the location various loactions of the IPs<br/>
<img src="https://i.postimg.cc/7PM0T1rS/Screenshot-2024-12-16-223156.png" />
<br />
<br />
I used geostatic command for geographic data that can be view on a map<br/>
<img src="https://i.postimg.cc/VvSx2sw8/Screenshot-2024-12-16-223455.png" />
<br />
<br />
Here is the map view<br/>
<img src="https://i.postimg.cc/br3R0kWY/Screenshot-2024-12-16-223535.png" />
<br />
<br />
 I save the result of geostats of IPs as report<br/>
<img src="https://i.postimg.cc/x80RbtsF/Screenshot-2024-12-16-224423.png" />
<br />
<br />
Confirmation of created report page<br/>
<img src="https://i.postimg.cc/CLx33NFN/Screenshot-2024-12-16-224439.png" />
<br />
<br />
The view page of the created report<br/>
<img src="https://i.postimg.cc/90ZDChP6/Screenshot-2024-12-16-224514.png" />
<br />
<br />
Created an Alert query to trigger when an alert identify a string<br/>
<img src="https://i.postimg.cc/vZfsQtK6/Screenshot-2024-12-16-230527.png" />
<br />
<br />
Confirmation of created alert page<br/>
<img src="https://i.postimg.cc/9M83x8Ds/Screenshot-2024-12-16-230630.png" />
<br />
<br />
Creating a dashbord based on a query result<br/>
<img src="https://i.postimg.cc/CLWRPJDZ/Screenshot-2024-12-16-233137.png" />
<br />
<br />
Dashboard created <br/>
<img src="https://i.postimg.cc/90sQkF43/Screenshot-2024-12-16-233631.png" />
<br />
<br />
Created additional 3 dashboard and added it to the existing dashboard. Here is the result<br/>
<img src="https://i.postimg.cc/bv6DTPRP/Screenshot-2024-12-16-235253.png" />
<br />
<br />
I arrange the dashboard to make it look more organize.Here is the result<br/>
<img src="https://i.postimg.cc/rpYs4J8F/Screenshot-2024-12-16-235706.png" />

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
