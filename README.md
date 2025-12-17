*This project has been created as a part of the 42 curriculum by daxferna*

# Description
The **Net Practice** project focuses on learning how computer networking works.\
Consisting on 10 levels, it presents students with incorrectly configured network diagrams that they must fix.\
The purpose of the project is to introduce the student to concepts such as TCP/IP addressing, routers and switches or gateways.
# Instructions
Once the tar file attached to the project's page has been downloaded and extracted, you have to run the `index.html` file.\
This file will prompt an interface in which you can choose between practice and evaluation mode. You should enter your intra login in order for the configuration files to be correct.\
The interface will show clues on why the configuration is not working on the bottom right.\
Once a level has been completed, a configuration file must be exported by clicking `Get my config`. The student has to submit 10 configuration files corresponding to each exercise, which will be placed at the repository root.\
During the evaluation, the student has to fix 3 random network diagrams in 15 minutes or less.
# Resources
### Concepts

- **IP Address:** \
	Identifier for a computer or device on a network. It makes possible the communication between devices.\
	Format: 4 octets of bits (0-255).\
	For example, `192.168.1.3`.\
	It consists of two parts:
	- Network address: number assigned to a network
	- Host address: number assigned to each host in that network
	To distinguish each part, we have to look at the **subnet mask**.

- **Subnet mask:** \
	IP-like address that lets you know which part of the IP is the network IP and which is the host IP.\
	It has also 4 octets of bits from 0 to 255 each\
	When converted to binary, the **ones** indicate the *network* and the **zeros** indicate the *host*\
	For example
	<pre>
	   255  .   255  .   255  .   0
	11111111.11111111.11111111.00000000</pre>
	means the first three octets identify the network address and the last one, the host address, so we have 254 available hosts (0 and 1 are reserved)\
	But in this one, it's trickier
	<pre>
	   255  .   255  .   240  .   0
	11111111.11111111.11110000.00000000</pre>
	the first 2 octets and the first part of the third octet are part of the network address.

When a device wants to communicate with another device within a network, it sends a broadcast to every device so the target identifies itself.\
This is easy in small networks, but when we have a large one, with many computers broadcasting at the same time, it leads to slow traffic and even a halt.\
Thats why networks need to be broken down into smaller ones, this is called subnetting and its possible thanks to routers, switches and subnet mask.
- **Routers:** \
	Devices that allow to subdivide a network.\
	If we have the subnet mask `255.255.255.0`, we can divide it in, lets say, 2 subnets, which can be 

- **Switches:** \
	text

- **TCP/IP Addressing:** \
	text

- **Default gateway:** \
	text

- **OSI layer:** \
	text
### Documentation
**- YouTube tutorials:** \
[Subnet mask](http://youtube.com/watch?v=s_Ntt6eTn94&list=PLCXqoZAc8-tzD5N5oCyIyEcMg_NDs6o7C)\
**- Articles** \
[Computer networks](https://www.freecodecamp.org/news/computer-networks-and-how-to-actually-understand-them-c1401908172d/)
### AI Usage
