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

Turning off Firewall to allow incoming attacks <br/>
<img src="https://i.imgur.com/PbuLVLd.png" height="80%" width="40%" alt="Open up Firewall"/>
<img src="https://i.imgur.com/bA6KHyz.png" height="80%" width="40%" alt="Firewall Off"/>
<br />
<br />

Virtual Machine under attack from multiple locations <br/>
<img src="https://i.imgur.com/MOYc8Pq.png" height="80%" width="80%" alt="Powershell ISE"/>
<br />
<br />

Geolocation API <br/>
<img src="https://i.imgur.com/eo48rh7.png" height="80%" width="80%" alt="Powershell ISE"/>
<br />
<br />

Code used to display info on map  <br/>
<img src="https://i.imgur.com/RL3tDlE.png" height="80%" width="80%" alt="Wolrd Map Code"/>
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
