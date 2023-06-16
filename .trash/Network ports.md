----
## Port 20, 21 – File Transfer Protocol (FTP)

This protocol is used to transfer files between systems, where users can connect to an FTP product and can view, upload, or download them. An example of usage would be a company using a server for file storage, where employees can connect via FTP and retrieve files.

----
## Port 22 – Secure Shell (SSH)

SSH allows users to connect to a remote host, such as a server if they have SSH open. This channel is encrypted, so any data moved between two connected systems will not be clearly visible. An example of usage would be an IT technician using SSH to connect to a server from their desktop to carry out maintenance.

---
## Port 23 – Telnet

This service was used before SSH and offers the same functionality, however Telnet does not use encryption, so the traffic can be captured and read by an attacker. Telnet should not be used due to this weakness, and SSH should always be implemented instead.

---
## Port 25 – Simple Mail Transfer Protocol (SMTP)

This protocol is used to send emails between servers within the network, or to external networks, such as over the internet. This is just a transport method, to actually download and view emails you need to use an email client and the protocol POP or IMAP.

---
## Port 53 – Domain Name System (DNS)

DNS operates on TCP and UDP ports 53 and uses relational databases to convert human-readable hostnames and domain names (such as Google.com) into their respective IP addresses so that communications can be sent to and from these hosts. The reason we use domain names is that they’re easy to remember. You remember securityblue.team, but you probably won’t remember 3.9.68.12!

---
## Port 67, 68 – Dynamic Host Configuration Protocol (DHCP)

DHCP is designed to assign IP address-related information to any hosts on the network automatically, such as the subnet mask and IP address. When you connect your phone to your network, it is being assigned an IP on the network because of dynamic host configuration protocol. DHCP uses 2 ports; UDP Port 67 and UDP Port 68.

---
## Port 80 – Hypertext Transfer Protocol (HTTP)

HTTP allows clients (browsers such as Chrome and Firefox) to connect to web servers and request content, which appears in the form of file downloads, web pages, and streaming services. So if you want to view the securityblue.team homepage, your browser will make an HTTP request to our web server, requesting to download the HTML web page. The server will respond with a 200 status code (which means “OK”, it has been successful) and then send the HTML page to the client, so you can view it on your screen. As HTTP is not encrypted, it is possible to conduct sniffing attacks, and see cleartext data as it is transmitted between the client and the server, such as passwords.

---
## Port 443 – Hypertext Transfer Protocol Secure (HTTPS)

HTTPS is a secure version of HTTP, and has the same functionality of retrieving content from web servers. However, the difference between the two is that HTTPS uses encryption to protect the transfer of data between a web server and a client. How do you turn HTTP into HTTPS? You need to use Transport Layer Security (TLS) formerly known as Secure Socket Layer (SSL). Sites that use HTTPS are less susceptible to man-in-the-middle and sniffing attacks.