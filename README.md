# networking-fundamentals

## A. OSI Model Summary

The **Open Systems Interconnection (OSI) model** is a conceptual framework used to understand how data travels across a network. It consists of seven layers, each performing a specific function to enable communication between devices and applications.

**7. Application Layer**  
It Provides network services to end-user applications, allowing programs to communicate over the network using protocols such as HTTP, FTP, SMTP and DNS.  
*Example:* Requesting a webpage in a browser using HTTP/HTTPS or sending an email via SMTP.

**6. Presentation Layer**  
It Formats, encrypts and compresses data to ensure it can be properly understood by the receiving system.  
*Example:* Streaming a video where the content is compressed into MP4 format or sending an encrypted message on WhatsApp.

**5. Session Layer**  
Manages communication sessions between devices, establishing, maintaining and terminating connections to ensure smooth data exchange.  
*Example:* Maintaining a video call session on Zoom or a multiplayer gaming session online.

**4. Transport Layer**  
Ensures reliable end-to-end communication by segmenting data, controlling flow and detecting errors. Protocols like TCP and UDP are used.  
*Example:* Downloading a file via TCP to ensure all data arrives correctly or streaming music via UDP for faster delivery even if some packets are lost.

**3. Network Layer**  
Handles logical addressing and routing so data can travel across different networks using IP addresses.  
*Example:* Routers forwarding packets from your computer to a website server or using a VPN where traffic is routed securely to a VPN server.

**2. Data Link Layer**  
Provides node-to-node communication within a local network using MAC addresses and performs error detection.  
*Example:* A laptop connecting to a Wi-Fi router using its MAC address or a switch delivering data frames to the correct device on a LAN.

**1. Physical Layer**  
Transmits raw bits over physical media, defining hardware components and signal types.  
*Example:* Sending data as electrical signals through Ethernet cables or as light signals through fiber-optic cables for internet connectivity.

---

## B. IP Subnetting Results (192.168.10.0/24)

- **IP Address:** 192.168.10.0  
- **Network Address:** 192.168.10.0  
- **Usable Host IP Range:** 192.168.10.1 – 192.168.10.254  
- **Broadcast Address:** 192.168.10.255  
- **Total Number of Hosts:** 256  
- **Number of Usable Hosts:** 254  
- **Subnet Mask:** 255.255.255.0  
- **IP Class:** C  
- **CIDR Notation:** /24  
- **IP Type:** Private  


## C. TCP/IP Protocol Suite in Action (Loading a Web Page)

When a user loads a webpage, the TCP/IP protocol suite operates across layers as follows:

1. **Application Layer:** The browser sends an HTTP/HTTPS request to the web server.  
2. **Transport Layer:** TCP divides the request into segments, ensures all segments are delivered reliably and in order.  
3. **Internet Layer:** IP adds source and destination IP addresses and routes the packets across networks to the server.  
4. **Network Access / Link Layer:** The packets are framed and transmitted over physical media (Ethernet, Wi-Fi) to reach the next network device.  

On the return trip, the web server’s response follows the same layers back to the client. TCP/IP ensures that the page loads correctly and completely, demonstrating reliable, layered communication between client and server.

