# Networking

## Network Components
A typical basic home network contains these components below:
- Modem
  - Modem is the **Internet Gateway**. It connects our home network to public internet.
- Router
  - Router allows networks connected to it to communicate with each other. In this case, it connects home network to public network
- Hub
  - Hub connects device connected to it. It broadcasts message sent from 1 device to all other devices connected to it
- Switch
  - Switch is a smarter hub. It is able to tell which device the message is directed to.
- NAT (Network Address Translation)
  - NAT is a method that translates private IP address into a public IP address. Usually it is a feature in a router.
  - In context of AWS, NAT or NAT gateway allows outbound internet connection without allowing inbound internet connection.

## DHCP vs Static vs DNS
- DHCP (Dynamic Host Configuratin Protocol) assigns an IP address from a pool of available ones to our computer automatically
- Static is assigning a fixed IP address to our computer
- DNS (Domain Name System): translates domain names (www.example.com) into IP addresses (10.10.10.10)
- DNS A Record: A table of domain name and its IP address. [Reference](https://www.cloudflare.com/learning/dns/dns-records/dns-a-record/)
- DNS CNAME Record: A table of domain's aliases and their mapped canonical domain name.

## OSI Layer
OSI is Open System Interconnection model. It is a framework that defines the function of networking / telco system.

- Layer 7: Application
  - Example:
    - Browser
    - Apps
- Layer 6: Presentation
  - deals with data conversion, encoding, compression, encryption
  - Example:
    - ASCII
    - JPEG
    - GIF
- Layer 5: Session
  - deals with opening/closing/managing session between end-user application
  - Example:
    - RPC - Remote Procedural Call
    - SOCKS
- Layer 4: Transport
  - deals with coordination of data transfer between host
  - Example:
    - TCP
    - UDP
- Layer 3: Network
  - deals with packet forwarding and routing
  - Example:
    - IP Address
- Layer 2: Data Link
  - provide node to node data transfer
  - Example:
    - MAC
- Layer 1: Physical
  - Example: Cable, Radio frequency


## TCP vs UDP
TCP:
- connection-oriented. establish connection between sender & receiver.
- data is guaranteed to be delivered. Will retry if undelivered
- data is delivered in the same order
- slower
- use case:
  - SSH
  - HTTP/S
  - FTP
  - SMTP

UDP:
- connection-less
- no guaranteed delivery
- no ordering in packet
- faster
- use case:
  - VPN tunnelling
  - gaming
  - live broadcasts / streaming

## IP Address & Subnet
- IP Address consists of 32-bit
- 32-bit comes from: dot separated 4 octets. 8bit.8bit.8bit.8bit
- Example:  
  - IP: 192.168.1.64
  - bits: 11000000.10101000.00000001.01000000 
- Subnet is a logical network within one single big network. In short it allows range grouping of allowed IP addresses within one single network.