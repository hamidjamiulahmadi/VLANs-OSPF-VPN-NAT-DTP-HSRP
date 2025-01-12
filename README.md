<h1>VLANs,OSPF,VPN,NAT,DTP,HSRP</h1>

<h2>Goal</h2>
<br />In the network that I am setting up, I will configure the Zurich network users to have access to the HQ servers, ensuring that users from the Zurich side can seamlessly connect to the Abu Dhabi servers.
Additionally, to ensure optimal connectivity, I will configure VLANs (Virtual Local Area Network), OSPF (Open Shortest Path First), VPN (Virtual Private Network), NAT (Network Address Translation), DTP (Dynamic Trunking Protocol), and HSRP (Hot Standby Router Protocol) in this lab environment.
<br />
Furthermore, I will deploy three routers—one for the Zurich side, one for the Internet ISP, and one for the HQ side—along with three servers, two distribution layer switches (one active and one standby for redundancy), four switches, three PCs, and three laptops. OSPF will be configured on the routers and distribution layer switches, while the ISP router will be configured with GRE (Generic Routing Encapsulation) to facilitate information transfer between the two sides. Additional details are provided in the accompanying diagram

<h2>Environments Used </h2>

- <b>Packet Tracer</b> 
- <b>Windows 11</b>

<h2>Lab walk-through:</h2>
Step Nr.1: The initial step involves creating a network diagram to provide a clearer understanding of the process and illustrate the methodology to be employed.
<p align="center">
Step Nr.1 : Network Diagram: <br/>
<img src="https://i.imgur.com/3bE6TBi.png" height="80%" width="80%" alt="Lab Steps Nr.1"/>
<br />
Step Nr.2: Here, I will allocate IP addresses to each PC, laptop, and server.
<p align="center">
Step Nr.2 : allocating IP addresses: <br/>
<img src="https://i.imgur.com/pXNb9My.png" height="80%" width="80%" alt="Lab Steps Nr.2"/>
<img src="https://i.imgur.com/iTWEGvE.png" height="80%" width="80%" alt="Lab Steps Nr.2"/>
<br />






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
