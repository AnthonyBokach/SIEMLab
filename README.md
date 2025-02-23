<h1>SIEM Lab - Elastic Stack</h1>

<h2>Description</h2>
Project focuses on creating an SIEM home lab by setting up an Elastic cloud instance and connecting it to a live virtual machine. The virtual machine is monitored for various security events and will be reported and analyzed with a custom dashboard in Elastic Stack to help visualize different events.
<br />


<h2>Languages and Utilities Used</h2>

- <b>C</b>
- <b>VM Workstation Pro 17</b>

<h2>Environments Used </h2>

- <b>Kali Linux OS</b>
- <b>Elastic Stack</b>

<h2>Project walk-through:</h2>

<h3>Elastic Stack SIEM Configuration and Management</h3>
<p align="center">
<b>Creating and deploying the Elastic cloud environment</b><br/>
<img src="https://i.imgur.com/hKmd2LW.png" height="80%" width="80%" alt="Deployed cloud environment"/>
<br />
Elastic has 3 different deployment options, each having specializations for various purposes. For this project, I went ahead and used the base deployment option (Elasticsearch) to understand how to configure Elastic Agents and forward data to the SIEM without extra tools. <br />
<br />
<b>Setting up Linux VM</b><br/>
<img src="https://i.imgur.com/UfUMbhC.png" height="80%" width="80%" alt="Linux VM"/>
<br />
For this project, Kali Linux was set up and deployed. While any other Linux OS would have worked for this project, Kali Linux was used due to the extensive features and tools that can be later used for other Cybersecurity projects. <br />
<br />
<b>Configuring and integrating Elastic Agent</b><br/>
<img src="https://i.imgur.com/CLq1Xw3.png" height="80%" width="80%" alt="Installing Elastic Agent"/>
<br />
In the context of this project, the Elastic agent is used to collect, log, and forward security-related events from the VM to the SIEM. <br />
<br />

<h3>Security Event Simulation and Analysis</h3>
<p align="center">
<b>Generating Security Events on VM</b><br/>
<img src="https://i.imgur.com/Y9ywgSS.png" height="80%" width="80%" alt="Reconnaissance-type commands"/>
<br />
A multitude of security-related events can be generated for the agent to collect and forward to our SIEM. This project used reconnaissance-type commands such as arp, id, uname, and hostname.  <br />
<br />
<b>Querying for Security Events in SIEM</b><br/>
<img src="https://i.imgur.com/9MobYRX.png" height="80%" width="80%" alt="Query page for process arguments"/>
<br />
By searching for specific logs related to the previously mentioned commands using process.args: "id" OR "uname" OR "arp" OR "hostname", we are able to get lots of important information regarding the details of the event. Data such as the timestamp, the name and arguments of the command, the user who executed the command, and more are readily accessible in each summary, which enables the concept of non-repudiation.  <br />
<br />

<h3>Visualization and Alerting in SIEM</h3>
<p align="center">
<b>Creating Dashboard for Data Visualization</b><br/>
<img src="https://i.imgur.com/I7gMCCo.png" height="80%" width="80%" alt="Graph of security events over time"/>
<br />
This project created a data visualization graph of security events over a given period. By having a live visual of how many events are occurring, we are able to interpret the information much better and allow individuals who don't understand the previously mentioned queries to follow along effectively. <br />
<br />
<b>Creating Security Alerts</b><br/>
<img src="https://i.imgur.com/BJYz7EI.png" height="80%" width="80%" alt="Recon Detection security alert"/>
<img src="https://i.imgur.com/U7pBkzb.png" height="80%" width="80%" alt="Recon Detection security alert email"/>
<br />
Security alerts are crucial for detecting security incidents and effective response times. This project sets up a security alert that notifies when reconnaissance-type commands are being used. <br />
<br />
</p>
<h2>Conclusion</h2>
<p><b>Elastic Stack SIEM Configuration and Management: </b>Successfully set up and configured Elastic Stack SIEM in a home lab environment. Demonstrated proficiency in deploying a Kali Linux VM, configuring Elastic Agents for log collection, and forwarding data to the SIEM for effective security event monitoring. </p>
<br />
<p><b>Security Event Simulation and Analysis: </b>Acquired hands-on experience in generating and analyzing security events using various reconnaissance commands on Kali Linux. Proficient in querying Elastic SIEM to identify and investigate security incidents, enhancing skills in network security monitoring and threat detection. </p>
<br />
<p> <b>Visualization and Alerting in SIEM: </b>Developed a custom dashboard in Elastic SIEM to visualize security events, demonstrating skills in data interpretation and pattern recognition. Successfully created and tested alert rules for detecting specific security events, showing competency in proactive incident response and alert management. </p>

<!--
<h3> Phase 1 </h3>
- Creating the VM
- Changing Firewall settings (Allow All)
- Creating a Log Analytics Workspace
- Connecting Log Analytics to VM
- Setting up Azure Sentinel
<h3> Phase 2 </h3>
- Turning off Windows Firewall in VM
- Creating the Powershell Script
- Getting Geolocation.io API Key
- Running Script
<h3> Phase 3 </h3>
- Setting up map in Sentinel using Latitude and Longitude
- 
--!>


<!--
 diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@

--!>
