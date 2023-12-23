# COMPUTER NETWORKS
3 Department Networks

# DEVICES USED:
•	60 Generic Computers
•	4 Routers (2911)
•	13 Switches (2960-24TT)
•	2 Generic Servers

# STRUCTURE:

The structure of the network comprises three departments: cybersecurity, artificial intelligence, and computer science. Within each department, there is a Lab, Faculty Office, and multiple Classrooms. While the actual labs have more than 25 computers, the model in this project represents each lab with 8 computers. Similarly, faculty offices are equipped with 7 computers, and each department includes 5 classrooms. Labs are connected to two switches, faculty offices to one switch, and the six classrooms within each department are linked to a single switch

![CN1](https://github.com/mishqatabid/Computer-Networks/assets/145700715/d7b1b5ad-1c19-41d4-b143-8090d8a90f6a)

# PROCEDURE:
First, add PCs to the topology and connect them with their respective switches. After performing this function, connect the switches with their respective routers. Now enter the CLI of the router and write the following set of commands to turn the DHCP in the PCs connected with the routers. Add the Respective IP range, subnet mask, default gateways, and respective DNS server IP. Now after writing the commands in the CLI of the routers, enter PC now go to Desktop > IP configuration and from here turn the DHP on. After this, you will observe that the IP is assigned to the computer from the given range, and the subnets and other blanks are assigned their values.

![CN2](https://github.com/mishqatabid/Computer-Networks/assets/145700715/a762eb9a-3e50-4039-9a4d-63213948c32a)
![CN3](https://github.com/mishqatabid/Computer-Networks/assets/145700715/b4aecd60-b4c9-4fc2-8d41-bd7a9b23292a)

Now set the servers. Firstly, assign the IPs, subnet masks, default gateways, and DNS server IP in the server configuration menu.

# DNS SERVER:
To set up the DNS server, follow these steps. 
Once you've assigned the IP address, navigate to Services > DNS, and enable the DNS option. Subsequently, input the server name in the Name tab and its IP in the IP Address tab. Additionally, click on the "Add" button below. If desired, you can include the IPs of the computers in this tab. To access the server, open PC > Desktop > Web Browser, and enter either the server's IP or its name. Upon doing so, a message indicating "WEB ACCESSED SUCCESSFULLY" will be displayed. You can also perform a ping to the server from PC > CMD using either the server's name or IP address.

![Screenshot 2023-12-23 121523](https://github.com/mishqatabid/Computer-Networks/assets/145700715/0cd85f3b-932c-402d-9182-7ed06a8622ab)
![CN4](https://github.com/mishqatabid/Computer-Networks/assets/145700715/d8edfb55-e271-4a54-a2fc-99fb79b98cd6)

# EMAIL SERVER:
Upon allocating the IP address, navigate to Services > EMAIL and enable the SMTP & POP options. Subsequently, include a domain in the Domain section, such as mail.com or Gmail.com. Proceed to add usernames and passwords in the designated sections and click the + button below. Additionally, integrate the domain name into your DNS server section. Then, access the CMD of a PC and input either the domain name or the server's IP to ping the server.

![CN5](https://github.com/mishqatabid/Computer-Networks/assets/145700715/9ead4ea7-7906-47b7-bcfe-aa938b2200e8)
![CN7](https://github.com/mishqatabid/Computer-Networks/assets/145700715/890cb52b-9fbc-414f-880c-b21c0a8e968e)
![CN6](https://github.com/mishqatabid/Computer-Networks/assets/145700715/cf44aaec-e8bc-46d4-93c7-aa17dcf599ef)

# ROUTING:
To start, incorporate serial ports from the Physical section into the routers. Utilize the Serial DCE Wire for interconnecting the routers as illustrated in the figure below. Proceed to assign IPs to the serial ports and select the checkbox located at the top right corner of the menu. Similarly, replicate this process for the remaining ports in each router. Next, navigate to the RIP section and input the addresses corresponding to the networks within the departments and the IPs of the routes, mirroring the configuration depicted in the figure below.

# SUBNETTING:
The provided IP addresses, namely 212.154.20.0, 212.154.21.0, 212.154.22.0, and 212.154.25.0, can be segmented into four subnets, each supporting a maximum of 64 IP addresses. This segmentation is achieved using a subnet mask of 255.255.255.192 or /26 in CIDR notation. The /26 mask allows for 2^6 or 64 potential host addresses per subnet, reserving 2 addresses for the network and broadcast addresses.<br>The subnet ranges and their assignable IP addresses are as follows:<br>The initial subnet spans from 212.154.20.0 to 212.154.20.63, with assignable IP addresses ranging from 212.154.20.1 – 212.154.20.62.<br>The second subnet range extends from 212.154.20.64 – 212.154.20.127, with assignable IP addresses spanning from 212.154.20.65 – 212.154.20.126.<br>Similarly, the third and fourth subnet ranges are 212.154.20.128 – 212.154.20.191 and 212.154.20.192 – 212.154.20.255, respectively.<br>By subdividing these IP addresses into subnets, network administrators can efficiently manage and allocate IP addresses, optimizing the utilization of the available IP address space.

# CALCULATIONS:
Ips used: 212.154.20.0, 212.154.21.0, 212.154.22.0, 212.154.25.0
<br>Number of Networks: 2^2 = 4
<br>Number of Hosts: 2^6 = 64
<br>Number of IPs: 2^6 – 2 = 62
<br>Network Bits for Class C: 11111111.11111111.11111111.11000000
<br>Subnet Mask: /26

# TABLE:

| Range                           | Assignable IPs                  |
|---------------------------------|---------------------------------|
| 212.154.20.0 – 212.154.20.63    | 212.154.20.1 – 212.154.20.62    |
| 212.154.20.64 – 212.154.20.127  | 212.154.20.65 – 212.154.20.126  |
| 212.154.20.128 – 212.154.20.191 | 212.154.20.129 – 212.154.20.190 |
| 212.154.20.192 – 212.154.20.255 | 212.154.20.193 – 212.154.20.254 |





