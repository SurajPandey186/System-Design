# 🌐 Networking Protocols -- Notes

## 📌 What is a Network Protocol?

A **Network Protocol** is a set of rules that define how data is
transmitted, formatted, and received between devices over a network.
These protocols ensure reliable communication between computers,
servers, routers, and other network devices.

Without protocols, devices would not understand how to send or interpret
data.

------------------------------------------------------------------------

# 🧠 Why Network Protocols Are Important

Network protocols help in: - Standardizing communication between
devices - Ensuring reliable data transmission - Managing network
traffic - Providing security - Enabling interoperability between
different systems

Example: When you open a website, several protocols work together to
deliver the webpage to your browser.

------------------------------------------------------------------------

# 📚 Types of Networking Protocols

## 1️⃣ Communication Protocols

### HTTP (HyperText Transfer Protocol)

-   Used for transferring web pages
-   Works on **port 80**
-   Stateless protocol

Example: Browser → HTTP Request → Web Server\
Web Server → HTTP Response → Browser

------------------------------------------------------------------------

### HTTPS (HyperText Transfer Protocol Secure)

-   Secure version of HTTP
-   Uses **SSL/TLS encryption**
-   Works on **port 443**
-   Protects sensitive data like passwords and payments

------------------------------------------------------------------------

### FTP (File Transfer Protocol)

-   Used to transfer files between computers
-   Works on **port 21**
-   Often used for uploading websites to servers

------------------------------------------------------------------------

### SMTP (Simple Mail Transfer Protocol)

-   Used for **sending emails**
-   Works on **port 25 or 587**

Flow: Email Client → SMTP Server → Recipient Mail Server

------------------------------------------------------------------------

### IMAP (Internet Message Access Protocol)

-   Used for receiving emails
-   Emails remain stored on the server
-   Allows access from multiple devices
-   Port: **143**

------------------------------------------------------------------------

### POP3 (Post Office Protocol v3)

-   Used for receiving emails
-   Downloads emails to the local device
-   Port: **110**

------------------------------------------------------------------------

# 🌍 Core Internet Protocols

## TCP (Transmission Control Protocol)

TCP ensures **reliable communication**.

Features: - Connection-oriented - Error checking - Guaranteed packet
delivery - Packet ordering

### TCP 3-Way Handshake

Client → SYN\
Server → SYN-ACK\
Client → ACK

------------------------------------------------------------------------

## UDP (User Datagram Protocol)

UDP is a **faster but less reliable protocol**.

Features: - Connectionless - No packet verification - Low latency

Used for: - Video streaming - Online gaming - VoIP calls

------------------------------------------------------------------------

## IP (Internet Protocol)

Responsible for **addressing and routing packets** across networks.

### IPv4 Example

192.168.1.1

### IPv6 Example

2001:0db8:85a3:0000:0000:8a2e:0370:7334

------------------------------------------------------------------------

# 🔧 Supporting Network Protocols

## DNS (Domain Name System)

DNS converts domain names into IP addresses.

Example: google.com → 142.250.183.14

------------------------------------------------------------------------

## DHCP (Dynamic Host Configuration Protocol)

Automatically assigns IP addresses to devices in a network.

Example: Router → Assigns IP → Laptop

------------------------------------------------------------------------

## ARP (Address Resolution Protocol)

Maps: IP Address → MAC Address

Example: 192.168.1.5 → 00:1A:2B:3C:4D:5E

------------------------------------------------------------------------

## ICMP (Internet Control Message Protocol)

Used for **network diagnostics and error reporting**.

Example: ping google.com

------------------------------------------------------------------------

# 🧩 Protocols in the OSI Model

  OSI Layer     Protocol Examples
  ------------- -------------------
  Application   HTTP, FTP, SMTP
  Transport     TCP, UDP
  Network       IP, ICMP
  Data Link     Ethernet, ARP

------------------------------------------------------------------------

# 📊 TCP vs UDP

  Feature       TCP                   UDP
  ------------- --------------------- -------------------
  Reliability   High                  Low
  Speed         Slower                Faster
  Connection    Connection-oriented   Connectionless
  Use Case      Web, Email            Streaming, Gaming

------------------------------------------------------------------------

# 📝 Example: Loading a Website

When you open:

https://google.com

Protocols involved: 1. DNS resolves domain to IP 2. TCP establishes
connection 3. HTTPS secures communication 4. IP routes packets 5. HTTP
transfers webpage data

------------------------------------------------------------------------

# 🚀 Key Takeaways

-   Network protocols define communication rules between devices.
-   Multiple protocols work together to enable internet communication.
-   TCP ensures reliability while UDP focuses on speed.
-   DNS translates domain names into IP addresses.
-   HTTP/HTTPS enable web communication.

------------------------------------------------------------------------

# 📚 Important Protocols to Remember

-   HTTP / HTTPS
-   TCP / UDP
-   IP
-   DNS
-   DHCP
-   ARP
-   SMTP
-   FTP
-   ICMP
