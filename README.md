# incident-analysis-project
<h1>Security incident analysis using NIST Cybersecurity Frameworks (CSF)</h1>


<h2>Description</h2>
This project consists of a Security Incident analysis that was performed on a fictitious Security Incident using the National Institute of Standards and Technology (NIST) Cybersecurity Frameworks (CSF). This project is a part of the graded courses in my Google Cybersecurity Certification course.
<br />


<h2>Framework used</h2>

- <b>National Institute of Standards and Technology (NIST) Cybersecurity Frameworks (CSF)</b> 


<h2>Scenario:</h2>

<p align="center">
Scenario: <br/>
<img src="https://i.imgur.com/5HJeesB.png" height="80%" width="80%" alt="Scenario"/>
<br />
<br />
Five core functions of the Framework:  <br/>
<img src="https://i.imgur.com/7ZSsLhz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<h2>Incident report analysis using the NIST CSF Frameworks</h2>
<h3>Summary of the Incident</h3>
The company experienced an outage of internal network resources. For a period of 2 hours, the internal network was out of service and this hindered usual business activities. Upon analysis, it was found that the server was flooded with ICMP requests and this caused the server to crash since it was out of ports. It is believed that the ICMP requests were coming from a malicious actor and this is the primary reason for the outage of the internal network.<br />
<h3>Identify</h3>
Using a packet sniffer or a network analyzer tool, the incident response team identified that the reason for the server crashing out is because of Distributed Denial of Service (DDoS) attack by flooding the server  ICMP packets. The team also identified that this was possible because the firewall was unconfigured and no rules were set to prevent the high number of incoming ICMP packets.<br />
<h3>Protect</h3>
The team has implemented a new firewall rule to protect the network by limiting the number of ICMP packets that can be received by the server. The team also installed Network Monitoring Software to detect any abnormal traffic patterns.<br />
<h3>Detect</h3>
To detect unauthorized ICMP requests the team has installed an Intrusion Detection System (IDS) that will filter out ICMP traffic based on any suspicious characteristics. The firewall also has a rule that will check the source IP address to protect against IP spoofing.<br />
<h3>Respond</h3>
The team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. Network security was hardened by implementing stricter firewall rules, implementing abnormal packet detection systems and applications.<br />
<h3>Recover</h3>
To recover from an ICMP Flooding DDoS attack, the network services will need to be restored to a normal functioning state. Firstly, the firewall will block any suspicious ICMP packets. Then the Critical Network services will need to be restored first. Lastly, once ICMP packets have timed out, the non-critical network services can be brought back online.<br />



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
