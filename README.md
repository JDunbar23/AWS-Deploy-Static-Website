<h1>Deployed an AWS hosted static Website</h1>

<h2>Description</h2>
Deployed my portfolio website located on my Github repository using AWS. I created a 3 tier VPC and the appropriate Security Groups to keep the app secure, launched the website in an EC2 instance using code to pull through the github repository. Finally bought and registered a domain for the website and secured it.
<br />
Created the infastructure to support databases being added to the private subnets in future.
<br />


<h2>Services Used</h2>

- <b>AWS</b>
- <b>VPC</b> 
- <b>EC2</b>
- <b>Route 53</b> 
- <b>Apache</b>


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

Created the NAT Gateways <br/>
<img src="https://i.imgur.com/GF1Rzbf.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Created the Private Route Table and assigned Private Subnets <br/>
<img src="https://i.imgur.com/iacERqC.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Created App Load Balancer Security Group <br/>
<img src="https://i.imgur.com/BUKUCYX.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Created SSH Security Group <br/>
<img src="https://i.imgur.com/4r7xzSq.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Created Webserver security group <br/>
<img src="https://i.imgur.com/iDQKx59.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Created Key pair + Created EC2 Webserver Instances for AZ1 and AZ2 <br/>
<img src="https://i.imgur.com/BaTyWH0.jpg" height="70%" width="70%" alt=""/>

<img src="https://i.imgur.com/Y3UiHWx.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Added this script to launch my website in the EC2 instances <br/>
<img src="https://i.imgur.com/yXfR9rE.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Created App Load Balancer <br/>
<img src="https://i.imgur.com/m9FQlAJ.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Can now view my website in the ALB DNS <br/>
<img src="https://i.imgur.com/VL4S6f7.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Registering my domain on Route 53 <br/>
<img src="https://i.imgur.com/iSl6GOM.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Assigned ALB onto Domain <br/>
<img src="https://i.imgur.com/TObzexu.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Requested SSL certificate for domain <br/>
<img src="https://i.imgur.com/Mj7L05g.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Assigned SSL certificate to ALB <br/>
<img src="https://i.imgur.com/s2QxPeh.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Redirecting traffic to secure port 443 <br/>
<img src="https://i.imgur.com/rpmspDK.jpg" height="70%" width="70%" alt=""/>
<br />
<br />

Website launched and secured <br/>
<img src="https://i.imgur.com/FmT8KeH.jpg" height="70%" width="70%" alt=""/>
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
