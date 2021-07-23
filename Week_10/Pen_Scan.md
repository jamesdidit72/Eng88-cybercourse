# Pen Scanning
## What is scanning?
Scanning is a set of procedures for identifying live hosts, ports, and services, discovering OS and architecture of target system, identifying vulnerabilities and threats in the network
## Network Scanning
- is the process of gathering information about a network to determine all active devices on it
- many types of network scanning:
    - passive scanning
    - active scanning
## Passive Scanning
- a passive scan silently analyses network traffic (packet sniffing) to identify endpoints and traffic patterns
    - TCPDump and Wireshark are passive network scanners
- has limitations
  - doesnt detect devices of applications that don't communicate
  - infected systems intentionally distributing misinformation
    
## Active scanning
- works by sending test traffic into the network and querying individual endpoints
- important measure in pen testing and hacking
- important to get an overview of whats happening
- two levels of active scanning
    - Host
      - involves detecting all active hosts on a network and mapping them to their IP addresses
      - Address Resolution Protocol (ARP) (getting an mac address from an IP from a PC on your network) scans: ARP requests can be sent out to many IP addresses on a LAN to determine which hosts are made up based on the ones that respond with an ARP reply
      - Internet Control message Protocol (ICMP)(pinging a device) scans: types of ICMP packets can be used
      - Echo (or ping) requests are used to detect if another host can be reached  
      - Address mask requests are intended to discover the subnet mask in use on the network  
    - Port
      - the process of sending packets to specific ports on a host and analysing the response to learn details about its running services or potential vulnerabilities
      - port scanning attempts to classify ports into one of three designations:
        - Open: the destination responds
        - Closed: the destination received the request packet but responded with a reply indicating that there is no service listening at the port
        - filtered: no reply is received
      - Port scanning methodologies:
        - vanilla: scan all known 65,535 ports
        - strobe: scan only known services/ ports
        - sweep: scan same port(s) on several machines
### OS fingerprinting
- process of determining the operating system used by a host on a network
- common techniques are based on analysing:
  - IP TTL (time to live) values (different OS assign different values to ongoing packets)
  - The IP DF Option
  - The IP Type of Service (TOS) (to give priority to packets over other packets)
  - IP ID values (IPID sampling)
  - CP window size
  - TCP Options (generally, in TCP SYN and SYN+ACK packets)  
### TCP Handshake
a single connection is established through a three way handshake, a packet is sent to a tcp port

SYN scan is the most common form of TCP scanning

ACKSCAN is used to determine if a port is filtered or not (used to probe the rues of a firewall)

TCP connect Scan (high level method of scanning) tries to connect to a port using tcp, will connect using all fo them?

NULL, FIN and Xmas Scans
- each results in either:
    - closed ports: a RST (or ICMP port  unreachable) packet
    - Open or filtered port: No response
IDLE scanning    
### UDP scanning
- UDP scans send a UDP packet to various ports on a target system and evaluate the response to determine availability of the service and the host
- Receiving a UDP packet in response indicates that the port is open

### Hybrid Scanning
- utilising both active and passive scanning together is important to gain an overview of the processes in the networks and to stop cyber threats
- it's important to be aware

### network mapper (nmap)
