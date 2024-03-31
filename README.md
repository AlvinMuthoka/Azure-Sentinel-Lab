# Azure-Sentinel-Lab

<h1>Failed RDP Attempts to IP Geolocation Information Threat Map Home Lab</h1>

<h2>Description</h2>
<b>The Powershell script in this repository parses out Windows Event Log information for failed RDP attacks integrates a third party API to collect geographic information on the attackers location.
</b>
<br />
<br />
The script is used in this home lab where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine hosted ion Azure acting as a honey pot.
I left the honeypot open for 3 days to observe live attacks (RDP Brute Force) from all around the world. A custom PowerShell script looks up the attackers geolocation information and plots it on a threat map in Sentinel!
<br />
<br />

<p align="center">
<img src="https://i.imgur.com/f5ziXry.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extracts RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>World map of incoming attacks after 72 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://i.imgur.com/nbHhV0J.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<p align="center">
<img src="https://i.imgur.com/D5TriUW.jpg" height="85%" width="85%" alt="Image Analysis Dataflow"/>
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
