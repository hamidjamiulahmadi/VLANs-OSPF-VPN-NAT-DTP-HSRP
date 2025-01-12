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
Step Nr.3: Subsequently, I will configure VLANs on the access switches, as illustrated in the diagram.
<p align="center">
Step Nr.3 : configuration of VLANs: <br/>
<img src="https://i.imgur.com/Wb1f5eA.png" height="80%" width="80%" alt="Lab Steps Nr.3"/>
<img src="https://i.imgur.com/gOkazbh.png" height="80%" width="80%" alt="Lab Steps Nr.3"/>
<br />
Step Nr.4: Next, I will configure DTP (Dynamic Trunking Protocol) on the distribution layer switches.
<p align="center">
Step Nr.4 : configuration of DTP: <br/>
<img src="https://i.imgur.com/G2955D9.png" height="80%" width="80%" alt="Lab Steps Nr.4"/>
<img src="https://i.imgur.com/FCsWB7I.png" height="80%" width="80%" alt="Lab Steps Nr.4"/>
<br />
Step Nr.5: Next, I will create VLANs and configure SVIs (Switched Virtual Interfaces) on the distribution layer switches.
<p align="center">
Step Nr.5 : configuration of VLANs, SVI: <br/>
<img src="https://i.imgur.com/4XsIXLm.png" height="80%" width="80%" alt="Lab Steps Nr.5"/>
<img src="https://i.imgur.com/ki4U1Hw.png" height="80%" width="80%" alt="Lab Steps Nr.5"/>
<img src="https://i.imgur.com/RRksgCI.png" height="80%" width="80%" alt="Lab Steps Nr.5"/>
<br />
Step Nr.6: Next, I will configure HSRP (Hot Standby Router Protocol) on the distribution layer switches.
<p align="center">
Step Nr.6 : configuration of HSRP: <br/>
<img src="https://i.imgur.com/twJhisx.png" height="80%" width="80%" alt="Lab Steps Nr.6"/>
<img src="https://i.imgur.com/6dt7nOb.png" height="80%" width="80%" alt="Lab Steps Nr.6"/>
<img src="https://i.imgur.com/KeMkKem.png" height="80%" width="80%" alt="Lab Steps Nr.6"/>
<br />
Step Nr.7: Here, I will configure the IP addresses between the distribution layer and the core layer. First, I will configure the distribution layer switch, followed by the configuration of the Zurich router.
<p align="center">
Step Nr.7 : configuration between distribution layer and core layer: <br/>
<img src="https://i.imgur.com/ID3E0aC.png" height="80%" width="80%" alt="Lab Steps Nr.7"/>
<img src="https://i.imgur.com/YVb6uhX.png" height="80%" width="80%" alt="Lab Steps Nr.7"/>
<img src="https://i.imgur.com/5ULt5EQ.png" height="80%" width="80%" alt="Lab Steps Nr.7"/>
<br />
Step Nr.8: Next, I will configure the router's internet interfaces and proceed to create a second loopback IP address.
<p align="center">
Step Nr.8 : configuration interfaces and proceed to create loopback IP: <br/>
<img src="https://i.imgur.com/kgYdtF0.png" height="80%" width="80%" alt="Lab Steps Nr.8"/>
<br />
Step Nr.9: Next, I will configure the OSPF routing protocol between the distribution layer switch and the Zurich router. I will begin by configuring OSPF on the distribution switch and include all VLANs within the OSPF area.
<p align="center">
Step Nr.9 : OSPF configuration: <br/>
<img src="https://i.imgur.com/ZcfGfS3.png" height="80%" width="80%" alt="Lab Steps Nr.9"/>
<img src="https://i.imgur.com/hzH2oR2.png" height="80%" width="80%" alt="Lab Steps Nr.9"/>
<img src="https://i.imgur.com/TNDRvNU.png" height="80%" width="80%" alt="Lab Steps Nr.9"/>
<img src="https://i.imgur.com/FljfBf4.png" height="80%" width="80%" alt="Lab Steps Nr.9"/>
<br />
Step Nr.10: The next step involves configuring NAT to enable user access to the internet. I will begin by defining a default route on the Zurich Router towards the internet router. Following that, I will configure an access control list to translate the VLAN range from 10 to 30, and set up NAT for both the outside and inside networks to ensure user access to the internet.
<p align="center">
Step Nr.10 : NAT configuration: <br/>
<img src="https://i.imgur.com/XBczpFe.png" height="80%" width="80%" alt="Lab Steps Nr.10"/>
<img src="https://i.imgur.com/5AByp3P.png" height="80%" width="80%" alt="Lab Steps Nr.10"/>
<img src="https://i.imgur.com/Ze35TIt.png" height="80%" width="80%" alt="Lab Steps Nr.10"/>
<br />
Step Nr.11: Next, I will configure the headquarters (HQ) and Abu Dhabi office side. I will begin by assigning the necessary IP addresses to the router interfaces, followed by configuring NAT. Subsequently, I will set up the default route and, finally, configure the access list on the router.
<p align="center">
Step Nr.11 : HQ Side configuration: <br/>
<img src="https://i.imgur.com/c3qVkt5.png" height="80%" width="80%" alt="Lab Steps Nr.11"/>
<br />
Step Nr.12: The next step is to establish a reliable connection between the Zurich side and the servers in Abu Dhabi. To achieve this, I will configure a VPN on the Zurich router's public IP and the Abu Dhabi router to ensure connectivity between the two sites.
<p align="center">
Step Nr.12 : VPN configuration: <br/>
<img src="https://i.imgur.com/G3GuQhC.png" height="80%" width="80%" alt="Lab Steps Nr.12"/>
<img src="https://i.imgur.com/iOTFslk.png" height="80%" width="80%" alt="Lab Steps Nr.12"/>
<br />
Step Nr.13: Next, I will configure OSPF on the tunnel interfaces of both routers to exchange routing prefixes and establish connectivity between them.
<p align="center">
Step Nr.12 : OSPF configuration on tunnel interfaces: <br/>
<img src="https://i.imgur.com/DRqU1Sp.png" height="80%" width="80%" alt="Lab Steps Nr.12"/>
<br />
Last Step: The final step is to verify that the servers have access to the ISP internet connection, and that users can access the servers. As demonstrated, both sides are successfully connected, and the lab setup is completed successfully.
<p align="center">
Last step : Connectivity and accomplishment: <br/>
<img src="https://i.imgur.com/s087YuW.png" height="80%" width="80%" alt="Lab Steps Nr.12"/>
<img src="https://i.imgur.com/5jMrmYZ.png" height="80%" width="80%" alt="Lab Steps Nr.12"/>
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
