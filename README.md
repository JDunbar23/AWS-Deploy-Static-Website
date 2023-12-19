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
<img src="https://i.imgur.com/bwmPltR.jpg" height="60%" width="60%" alt=""/>
<br />
<br />

Turn on DNS Host names <br/>
<img src="https://i.imgur.com/ojRn8UG.jpg" height="60%" width="60%" alt=""/>
<br />
<br />

Creating an Internet Gateway and attaching it to the VPC <br/>
<img src="https://i.imgur.com/5UFyvu1.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Creating the Public Subnets  <br/>
<img src="https://i.imgur.com/JQ2UCHA.jpg" height="50%" width="50%" alt=""/>
<br />
<img src="https://i.imgur.com/FrsFxMr.jpg" height="50%" width="50%" alt=""/>
<br />
<br />

Enable Auto Assign IPv4 Addresses on the Public Subnets <br/>
<img src="https://i.imgur.com/iUMAugX.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Creating the Public Route Table <br/>
<img src="https://i.imgur.com/KqZBxCV.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Assign the Public Subnets to the Public Route Table <br/>
<img src="https://i.imgur.com/TzQukcQ.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Created the Private Subnets for the project <br/>
<img src="https://i.imgur.com/frR4e0h.jpg" height="70%" width="70%" alt=""/>
<br />
<br />



Enable Auto Assign IPv4 Addresses <br/>
<img src="https://i.imgur.com/iUMAugX.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Enable Auto Assign IPv4 Addresses <br/>
<img src="https://i.imgur.com/iUMAugX.jpg" height="70%" width="70%" alt=""/>
<br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
