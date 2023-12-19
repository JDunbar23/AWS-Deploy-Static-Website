<h1>Deployed an AWS hosted static Website</h1>

<h2>Description</h2>
The PowerShell script contained within this repository is designed to extract data from Windows Event Logs regarding unsuccessful RDP intrusion attempts. It then employs a third-party API to gather geographical data related to the origin of the attackers.
<br />
<br />
This script is utilized in the context of my Azure Sentinel configuration, where it is connected to a live virtual machine serving as a decoy for potential cyberattacks. I have personally witnessed live attacks, particularly RDP brute force attacks, originating from various locations worldwide. To visualize this information, I utilized a custom PowerShell script to retrieve the geographic information of the attackers and visualize it on an Azure Sentinel map.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Microsoft Azure</b>
- <b>Virtual Machine</b> 
- <b>Windows 10</b>
- <b>Azure Sentinel</b> 
- <b>PowerShell: Extract RDP failed logon logs from Windows Event Viewerl</b> 
- <b>ipgeolocation.io: IP Address to Geolocation API</b>


<h2>Walkthrough</h2>

Creating the VPC for the project <br/>
<img src="https://i.imgur.com/bwmPltR.jpg" height="100%" width="40%" alt=""/>
<br />
<br />

Turn on DNS Host names <br/>
<img src="https://i.imgur.com/ojRn8UG.jpg" height="50%" width="80%" alt=""/>
<br />
<br />

Creating an Internet Gateway and attaching it to the VPC <br/>
<img src="https://i.imgur.com/5UFyvu1.jpg" height="80%" width="80%" alt=""/>
<br />
<br />

Creating the Public Subnets  <br/>
<img src="https://i.imgur.com/JQ2UCHA.jpg" height="30%" width="80%" alt=""/>
<br />
<img src="https://i.imgur.com/FrsFxMr.jpg" height="30%" width="80%" alt=""/>
<br />
<br />

<h2>World Map of incoming attacks</h2>
<img src="https://i.imgur.com/i9mCBAv.png" height="80%" width="80%" alt="Azure Attack Map"/>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
