# <h1>Virtual DHCP Server Deployment Using Windows Server 2019</h1>

<h2>Description</h2>

<p>In this project, I used Oracle VirtualBox to create a virtualized network environment. I deployed a Windows Server 2019 virtual machine and configured it as a DHCP server. A separate Windows 10 virtual machine was then connected to the same virtual network to verify dynamic IP address allocation. This setup demonstrated my ability to create and manage network services in a virtualized environment, as well as my understanding of DHCP configuration and client-server communication within Windows-based systems.</p2>

<img width="829" height="772" alt="image" src="https://github.com/user-attachments/assets/824f3e3f-402e-4f0e-a3e2-8a5fa1d579c5" />



Components used:

Windows Server 2019 (Domain Controller):

Deployed as a DHCP server and configured with two network interfaces:

NIC 1 (External): Connected to the home router to obtain an IP address via DHCP for internet access.

NIC 2 (Internal): Static IP address (172.16.0.1) to serve the internal VirtualBox default gateway.

Configured Active Directory Domain Services (AD DS) to establish a domain: JTdomain.com.

Set up Routing and Remote Access (RAS) using NAT to enable internet connectivity for internal clients.

<h2>Domain/DHCP configuration</h2>
<p>https://youtu.be/JIZfHFkSMCs</p>

<h2>Adding the scope</h2>
<p>https://www.youtube.com/watch?v=Kkd4Nk6MSuk</p>






<br>



</br>





Windows 10 Client:

Configured with a single internal NIC.

Connected to the internal network and received an IP address from the DHCP server.

Successfully joined the JTdomain.com domain.

DHCP Scope Settings:

IP Range: 172.16.0.100 – 172.16.0.200

Subnet Mask: 255.255.255.0

Gateway: 172.16.0.1

DNS: 172.16.0.1

<h2>Client running on DHCP</h2>
<p>https://youtu.be/JsexRvPJH58</p>





<br>


</br>

Project Outcomes:

Demonstrated the ability to deploy and configure DHCP services in a Windows Server environment.

Successfully integrated a client machine into a domain and verified dynamic IP allocation.

Enabled domain-based network management and internet access via NAT routing.



<br>


</br>

Skills Demonstrated:

Virtualization using Oracle VirtualBox

DHCP server configuration

Active Directory domain setup

NAT and routing configuration via RAS

Internal network planning and IP management





