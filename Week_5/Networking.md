# Monday
## First recording (07/06/2021)
### What is a network
- A collection of devices that are connected to each-other
- Main idea is to be able to exchange data
Main Network components are the host/end device

Any device connected to the network that exchanges data is a host/ end device

Devices on the network that are assigned an address for communication purposes

Servers are a software providing a service to other devices on the network

Client is a device that requests for a service

Server client architecture, one requests (client), one provides (server)

Peer to peer, both can ask for services from each other
- Printer and pc is a peer to peer architecture

Intermediary devices connect the end devices to the network (wireless router, router, LAN switch, multilayer switch, Firewall Appliance)

In the network to connect the end devices or to provide a function to the end devices

Network media:
-	Metal wires (cable)
-	Fibre optics
-	Wireless (any)

Main four categories (host, server/client, intermediary devices, network media)

Network types:
-	Size of the area covered
-	Number of users connected
-	Type of services (provided by the network)
-	Area of responsibility ((LAN, your responsibility) (WAN, not your responsibility))
Most common networks
-	LAN (local area network)
o	Network in a small geographical area (house)
-	WAN (wide area network)
o	Network infrastructure that provides network connection over a large geographical location (internet (collection of WANs))
-	MAN (metro area network (basically a WAN))

Internet: (interconnected network (public)(worldwide))

intranet (private connection (company only))

- refers to a private connection of LANs and WANs in a company

extranet (not really used, not well defined (suppliers, customers collaborators))
- secure and safe access between different orgs

communication fundamentals:

formed of three elements
-	Message source (sender)
-	Message destination (receiver)
-	Channel

Goal = to transmit a message over the channel

Transmit the source message to the destination message over the channel

Message delivery options
-	Unicast (send message to one destination)
-	Multicast (multiple destinations)
-	Broadcast (all destinations)

## Second recording (07/06/2021)
Protocol suite/standards

A group of inter-related protocols, each one performs a specific task

Iso TCIP

Developed by ISO and ITU

OSI is a standard (the concept)

(picture is osi model layer (open systems interconnection))

Physical = physical attributes of the connection, uses network media, can find out network speeds here

Data link = layer that takes care of the protocols, describes methods of exchanging data between the protocols, where you define the network and physical addressing

Network = addressing and routing are the main functionalities of this layer, provides services to exchange data across networks Ips are on this layer, to give an address to the host, or any device on the network. Also determines the routing

Transport = Main protocols TCP (Transmission control protocol) reliable and ensures all data arrives at the destination (email)

Session = want to send data, creates a connection between the host and the client. Session is a connection between the sender and the receiver, goes through authentication, have to go through multiple parameters

UDP (User datagram protocol) similar transport layer, does not provide reliability or flow control but it is faster (streaming)

Session, presentation and application have been merged into one layer, Application

Related to the application and the software running
#### Ports numbers
Port numbers (range from 0 - 65535)(TCP and UDP use the same range)

65535 = 2^16 = 16 bits

Internet assigned number authority (IANA) incharge of number above.

0-1023 = well-known ports

1024- 49151 = registed ports

48152-65535 = dynamic ports

Bandwidth: Capacity that the media can carry data

Well-Known Port Numbers

Port |Number	Protocol|	Application|
|:---------: |:----------------------------: |:--------: |
20|	TCP|	File Transfer Protocol (FTP) – Data|
21|	TCP|	File Transfer Protocol (FTP) – Control|
22|	TCP	|Secure Shell (SSH)|
23|	TCP	|Telnet|
25|	TCP	|Simple Mail Transfer Protocol (SMTP)|
53|	UDP, TCP|	Domain Name Service (DNS)|
67|	UDP|	Dynamic Host Configuration Protocol (DHCP) – Server|
68|	UDP|	Dynamic Host Configuration Protocol – Client|
69|	UDP|	Trivial File Transfer Protocol (TFTP)|
80|	TCP|	Hypertext Transfer Protocol (HTTP)|
110|	TCP|	Post Office Protocol version 3 (POP3)|
143|	TCP|	Internet Message Access Protocol (IMAP)|
161|	UDP|	Simple Network Management Protocol (SNMP)|
443|	TCP|	Hypertext Transfer Protocol Secure (HTTPS)|


## Third recording (07/06/2021)
IP addressing:
Positional numeral system
# Fourth recording (07/06/2021)
MAC = Media Access Control (similar to a serial number)

48 bit number, first 6 characters represent the vendor, second 6 represent the NIC

NIC = Network interface Card (includes the Mac address)

Command prompt for MAC address = ipconfig /all

Network layer addressing:
IP (Internet protocol) address
- Ipv4
    - A series of 1s and 0s. 32 bits long. 4 octets (1 octets = 8 bits)
    - Represented as decimal
    - example
        - IP = 172.16.254.1
        - Binary = 10101100.00010000.11111110.00000001
        - 32 bits, 4 octets

You need to know if 2 devices are in the ame network or not, by comparing their network ID

They are put into classes to determine if theyre in the same network

## Fifth recording (07/06/2021)

If an IP includes /number

The number of 1s in the subnet mask, which is the network address

Subnet mask

network can be 1,2 or 3 octets, the rest is host

series of 1s, followed by a series of 0s

1s represent the network ID

0s represent the host ID

The first address in the network is the network address

# Tuesday

## First recording (08/06/2021)

Every machine has a unique IP address

Summary of last session (octets, classes)

Network Id
- First IP in the network
- Couldnt be allocated to any machine on the network
- All hosts should have the same network ID
- If they have different network ID, theyre on different networks
    - Usually abbreviated by: NetID
- To calculate use AND rather than class

Subnet mask
- is a 32-bit address used to mask a portion of the IP address to distinguish the network ID from the host ID
- Each host on a TCP/IP network requires a subnet mask
- Networks are not divided into subnets
- Two forms
    - Type one: 255.255.0.0 = 16 1s
    - Type two: IP/16 = 16 ones
Broadcast:
- Last IP in the network
- All hosts bits of the IP address will be 1s
- Cant be allocated
    - Usually abbreviated by: bcastID

## Second recording (08/06/2021)
A switch work on the data link, doesn’t understand IP addresses, understands MAC addresses
ping is a tool that replies on a protocol called: ICMP (internet control messaging protocol)

ARP: Address resolution Protocol (gets the MAC address of the IP address)
## Third recording (08/06/2021)

Ipconfig is to find the ip of a device (windows)

Ifconfig for other OS

Ping messages:
- Reply indicates that there is a connection
- Timed out means the host did not receive a message back
- Host unreachable computer destination cannot be reached

A broadcast can never go behind a router

How to restrict the broadcast domain?
- Theyre restricted by routers (layer 3 devices)

A router is a computer that has two network cards, that can wire traffic between different networks. It is a level 3 device

A default gateway is where the traffic will be sent if the destination is not on your network

Keep the default gateway last IP value (192.168.1._) random for security

# Wednesday

## First Recording (09/06/2021)
IPS and MAC addresses belong to a host, but are assigned to an interface (NIC (network interface card))

DHCP (Dynamic host configuration protocol)

Application layer protocol

A server client protocol

Port 67/ udp for the server, post 68/ udp for the client

If a protocol is listening to a port then it is on the application layer

Clients have the config on a lease and have to renew their lease frequently, allows for changing the config from one location, also allows for the system to give the IP to a different client when the previous one is no longer available (when connected to free wifi, you have a lease on the config, if you leave, itll will make that connection available for other users)

- Ipconfig commands
- Ipconfig- shows the ip
- Ipconfig /all
- Ipconfig /renew – renews the lease on the config
- Ipconfig /release – releases the config

http (hyper-text transfer protocol) app layer protocol (works on TCP 80)

https (^^^ secure) (port 403)

html (hyper-test markup language)

FTP (file transfer protocol) (uses port 20 and 21) client server protocol

- They use 2 port number because one is used for the control (20)(establish the connection between the client and the server), and the other is used to transfer the data (21)

Protocols are organised by DNS (domain name system) converts host and domain names into ip addresses
- Uses port 53 udp
## Second recording (09/06/2021)

A firewall is a system or group of systems that enforces access control policy between networks to protect the network

They share common properties

Can be hardware(basically a computer) or software(be installed anywhere)

Allows
- Traffic from any external address to the web server
- Traffic to FTP, SMTP, internal IMAP servers

Denys
- No inbound traffic
- MS domain broadcasts

Packet filtering firewall

Transport and network layer include ip, ports

Application gateway firewall, more capabilities than a normal firewall (works on network, transport, session and application)


Wildcard mask is the revserse of the subnet mask

De-militarized zone(DMZ, 50% secure) allows in and outbound traffic in from the internet (public, 0% secure), but doesn’t send anything to the private(our network, 100% secure) servers

On their own network

How to write a policy
- Access control list (ACL) contains the rules that grant or deny access to certain resource.
- Can only Grant or deny
- Filter the access to the resources

# Thursday & Friday

## First recording (10/06/2021)

Using the new VM box, “labtainer”

Password = password123

It is a lab using containers (same as docker containers)

Each component (firewall, pc, router) is in its own container


In VM, labtainer shows the available labs

Ctrl + c to stop a command

Iptables for firewalls

Labtainer LAB_NAME to start a lab

Stoplab to stop the labs, saves it in its current state

Labtainer -r LAB_NAME to restart a lab

Ifconfig for ip stuff

Sudo apt install net-tools, incase ifconfig isn’t installed

127.0.0.1 is the local host (the same machine)

route -n shows the ip routing table (includes destination, gateway and subnet mask)

ARP (address resolution protocol) used to broadcast for an IP address, which then will return a MAC address for that IP

Arp -n displays the gateway and the mac address

Ip address for the current interfaces

Sudo ip link set INTERFACE_NAME up/ down, to turn the interface on/ off

Sudo ifconfig INTERFACE_NAME up/ down, to turn the interface on/ off

Ifconfig -a to list all interfaces, on or off

Ip add show INTERFACE_NAME, shows a specific interface

Sudo ip address add NEW_IP/SUBNET_MASK (can be /24) device INTERFACE_NAME to add a IP to an interface

Sudo ifconfig INTERFACE_NAME NEW_IP netmask SUBNET_MASK to add a IP to an interface

Sudo ip address del IP/SUBNET_MASK dev INTERFACE_NAME deletes the ip from the interface

Sudo ip route add/del default via GATEWAY_IP to add/delete the default gateway

# Friday

## This day was spent practicing and completing labtainers


## First recording (11/06/2021)

VPN is a concept of creating a virtualised private network between two networks

VPN (virtualised private network)

VPN (Virtual Private Network) is to secure network traffic between sites and users, organisations use vpns to create an end to end private network connections

Creates a virtual connection across the internet that is encrypted

When using a vpn for professional purposes, it creates a secure IP for the host to talk to the main site which also has a secure VPN and the communication is encrypted

4 major protocols:

- Point to point tunnelling protocol (pptp)
- L2tp (layer to tunnelling protocol)
- Ipsec (internet protocol security)
- Ssl (secure socket layer)

Connection established through a router, data transfer through the vpn

Vpn gateway is not on the servers, just on the networks

Vpn server can run on a vpn gateway, a router and a firewall

To main functions, tunnelling and encryption

Tunnel connects the hosts to communicate

Encryption is used to hide the data whilst travelling through the tunnelling

Network address translation (NAT)

Helps with IP address shortages (IPv4)

Translates private address to public addresses

Can turn many private address on one network to one public address

Static nat happens on the router or firewall

Dynamic nat

Nat overload, putting loads of private addresses into ne public address

