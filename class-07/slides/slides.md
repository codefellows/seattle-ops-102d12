<!-- .element class="split-screen-with-title" -->

# Ops 102 Overview

<div>

<div>

  - Class 01: What is a computer? <!-- .element: class="fragment" data-fragment-index="1" -->
  - Class 02: Build a computer <!-- .element: class="fragment" data-fragment-index="2" -->
  - Class 03: Startup sequence and BIOS <!-- .element: class="fragment" data-fragment-index="3" -->
  - Class 04: Operating Systems <!-- .element: class="fragment" data-fragment-index="4" -->
  - Class 05: Install Virtualbox <!-- .element: class="fragment" data-fragment-index="5" -->

</div>

<div>

  - Class 06: SOHO Networking <!-- .element: class="fragment" data-fragment-index="6" -->
  - Class 07: Network Connectivity <!-- .element: class="fragment" data-fragment-index="7" -->
  - Class 08: Windows OS Virtualization <!-- .element: class="fragment" data-fragment-index="8" -->
  - Class 09: Basic Windows Operations <!-- .element: class="fragment" data-fragment-index="9" -->
  - Class 10: 201 Entrance Exam <!-- .element: class="fragment" data-fragment-index="10" -->

</div>

NOTE:
SAY:
- Here's where we are in the Ops 102 course curriculum.

---

<!-- .element class="split-screen-with-title" -->
# Agenda

<div>

<div>

- Review of previous class
- Remote Connectivity
- Network Protocols
  - TCP/IP Model
  - IP address configuration
- Network Ports
  - SSH
  - RDP
  - SCP
- Demo
- Lab

</div>

<div>

![Image](/ops-102-guide/curriculum/class-07/slides/assets/2_0.png)

</div>

</div>

NOTE:
SAY: Here's our plan for class today.

---

<!-- .element class="main-title" -->
# Review

- What did you learn?
- What did you struggle with?
- What blockers did you encounter?
- What fun or cool solutions did you come up with?

NOTE:
DO: Go around the class and let students talk about what they learned previous class.

---

<!-- .element class="split-screen-with-title" -->
# Our Lab Plan

<div>

<div>

- Access lab PC from personal computer
  - Secure Shell (SSH)
    - port 22
  - Secure Copy Protocol (SCP)
    - port 22
  - Microsoft Remote Desktop Protocol (RDP)
    - port 3389

</div>

<div>

![Image](/ops-102-guide/curriculum/class-07/slides/assets/lab07-topology.png)

</div>

</div>

NOTE:
SAY:
- SSH is used to establish a secure command-line interface connection between the personal computer and the lab PC.
  - It provides encrypted communication and secure remote access to the lab PC's command line.
- SCP is a secure file transfer protocol that operates over SSH.
  - It allows secure copying of files between the personal computer and the lab PC using the SSH infrastructure.
  - In other words, you can share files or transfer files from your personal computer to your lab PC.
- RDP is a proprietary protocol developed by Microsoft for remote desktop access to Windows-based systems.
  - By using port 3389, it enables your personal computer to establish a remote desktop session with your lab PC, providing a full control GUI connection to it.

---

<!-- .element class="split-screen-with-title" -->
# Network Protocols

<div>

<div>

- A protocol is a set of agreed upon rules to facilitate communication
  - The Internet Protocol (IP) facilitates the routing and addressing of data packets to reach their destination
  - An IP address is the “location” (mailing address) of a computer
- TCP-IP Model depicts four “layers” of computer networking

</div>

<div>

![Image](/ops-102-guide/curriculum/class-07/slides/assets/6_0.png)

</div>

</div>

NOTE:
SAY:
- A protocol is a set of agreed-upon rules to facilitate communication.
  - The Internet Protocol (IP) facilitates the routing and addressing of data packets to reach their destination.
    - IP is a fundamental protocol in computer networking that enables the identification and routing of data packets across a network or even the internet.
    - It defines how packets are addressed and delivered to their intended destinations.
  - An IP address is the "location" (mailing address) of a computer.
    - An IP address is a unique numerical identifier assigned to each device connected to a network.
    - It serves as the address of a computer or any other networked device, allowing it to send and receive data within the network or across the Internet.

- TCP/IP Model depicts four "layers" of computer networking.
  - The Application Layer
    - This layer represents the protocols and services that enable communication between applications running on different devices.
    - Examples include HTTP, FTP, Telnet, and DNS.
  - The Transport Layer
    - The transport layer provides reliable and efficient data transfer between devices.
    - It ensures that data packets are delivered without errors and in the correct order.
    - Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) are commonly used in the transport layer protocol.
  - The Internet Layer
    - The internet layer (also known as the network layer) handles the addressing, routing, and fragmentation of data packets across different networks.
    - The Internet Protocol (IP) operates at this layer.
  - The Link Layer
    - The link layer is responsible for the physical transmission of data over a network.
    - It deals with protocols that define how data is formatted, transmitted, and received on the physical network medium, such as Ethernet or Wi-Fi.

---

<!-- .element class="split-screen-with-title" -->
# IP Address Configurations

<div>

<div>

- A dynamic IP address is what most hosts receive from DHCP server when connecting to a network
  - Lease time
  - Can change (be “lost”)
- A static IP address is configured on the host itself
  - Never changes but can cause IP conflicts
- A reserved IP address is achieved by associating an IP address to a MAC address on the DHCP server

</div>

<div>

![Image](/ops-102-guide/curriculum/class-07/slides/assets/7_0.png)

</div>

</div>

NOTE:
SAY:
- A dynamic IP address is what most hosts receive from a DHCP server when connecting to a network.
  - Lease time
    - When a host receives a dynamic IP address from a DHCP (Dynamic Host Configuration Protocol) server, it is assigned a lease time.
    - The lease time represents the duration for which the IP address is valid and can be used by the host.
    - After the lease time expires, the host may need to renew the lease to continue using the same IP address.
  - Can change (be "lost")
    - Dynamic IP addresses are subject to change, as the DHCP server may assign different IP addresses to hosts over time.
    - This means that when a host reconnects to the network or after the lease expires, it may receive a different IP address.
    - As a result, the previously assigned IP address can be "lost."

- A static IP address is configured on the host itself.
  - Never changes but can cause IP conflicts
    - A static IP address is manually configured on the host by the user or network administrator.
    - Unlike dynamic IP addresses, a static IP address remains the same unless it is manually changed.
    - However, you want to watch out for IP conflicts, which can occur if multiple devices on the network are assigned the same static IP address.
    - Therefore, it is important to ensure that each device on the network has a unique static IP address.

- A reserved IP address is achieved by associating an IP address with a MAC address on the DHCP server.
  - By associating an IP address with a MAC address on the DHCP server, the DHCP server reserves a specific IP address for a particular device.
  - This ensures that when that device connects to the network, it will always receive the same IP address.
  - This association between the IP address and MAC address helps maintain consistent addressing and facilitates device identification on the network.

---

<!-- .element class="title-and-text" -->
<div>

# What is DHCP?

- DHCP stands for Dynamic Host Configuration Protocol.
- Client-server model
- Simplified overview of how DHCP works:
  - Discover
  - Offer
  - Request
  - Acknowledgment
  - Lease

</div>

NOTE:
SAY:
- DHCP stands for Dynamic Host Configuration Protocol.
  - It is a network protocol commonly used to automatically assign IP addresses and network configuration parameters to devices on a network.
- The DHCP protocol operates in a client-server model, where there is a DHCP server responsible for managing and allocating IP addresses and a DHCP client that requests and receives network configuration information.
- Here's a simplified overview of how DHCP works:
  - Discover
    - When a device connects to a network, it broadcasts a DHCP Discover message.
    - This message is sent out to locate a DHCP server on the network.
  - Offer
    - Upon receiving the DHCP Discover message, DHCP servers on the network respond with a DHCP Offer message.
    - This message contains an available IP address and other network configuration parameters, such as subnet mask, default gateway, and DNS server information.
  - Request
    - The device, acting as a DHCP client, selects one of the offered IP addresses and sends a DHCP Request message to the chosen DHCP server.
    - The Request message confirms the selection of the IP address and other offered parameters.
  - Acknowledgment
    - The DHCP server receives the DHCP Request message and sends a DHCP Acknowledgment message to the client.
    - This message confirms the allocation of the requested IP address and provides the client with the approved network configuration parameters.
  - Lease
    - The DHCP server assigns a lease time to the client, indicating the duration for which the client can use the assigned IP address.
    - Before the lease expires, the client can choose to renew the lease, ensuring it can continue using the same IP address.
    - If the lease is not renewed, the IP address may be released back to the DHCP server and made available for other devices.

---

<!-- .element class="split-screen-with-title" -->
# Network Ports

<div>

<div>

- Network ports are like numbered doorways into a computer system.
  - Every data packet must designate a source and destination port <!-- .element class="medium-text" -->
  - Open ports permits traffic <!-- .element class="medium-text" -->
  - Closed ports blocks traffic <!-- .element class="medium-text" -->
- Port numbers range from 0 to 65535.
  - Well-known ports (0-1023) are assigned and controlled. <!-- .element class="medium-text" -->
  - Registered ports (1024-49151) are not assigned or controlled, but can be registered to prevent duplication. <!-- .element class="medium-text" -->
  - Dynamic/private ports (49152-65535) are not assigned, controlled, or registered. <!-- .element class="medium-text" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-07/slides/assets/8_0.png)

</div>

</div>

NOTE:
SAY:
- Network ports are like numbered doorways into a computer system.
  - They enable communication between different devices and applications over a network.
- Every data packet must designate a source and destination port.
  - The source port is the port number from which the packet originates, while the destination port is the port number to which the packet is being sent.
- Ports can be either open or closed, much like doors.
  - An open port permits traffic, allowing data packets to flow in and out freely.
  - On the other hand, a closed port blocks traffic, preventing any data packets from passing through.
- Port numbers range from 0 to 65535.
  - Certain well-known ports have been assigned specific purposes by the Internet Assigned Numbers Authority (IANA), while others are available for general use.
- The well-known ports (0-1023) are reserved for commonly used services.
  - For example, port 80 is typically used for HTTP (Hypertext Transfer Protocol), port 443 for HTTPS (HTTP Secure), and port 25 for SMTP (Simple Mail Transfer Protocol).
- Registered ports (1024-49151) are used by applications that are not as widely recognized as the well-known ports.
  - These ports can be registered with IANA for specific purposes.
- Dynamic or private ports (49152-65535) are available for temporary use by applications and are assigned dynamically by the operating system.

---

<!-- .element class="split-screen-with-title" -->
# SSH

<div>

<div>

- Secure Shell (SSH) is a modern standard for remote terminal access.
  - Text-only, no GUI
  - SSH can use password authentication to establish a terminal-only connection to a computer running the SSH service
- Requires port 22 to be open on the "server"
- Many applications such as WinSCP and VSCode can "piggyback" SSH by using it as a background means of transferring data

</div>

<div>

![Image](/ops-102-guide/curriculum/class-07/slides/assets/9_0.png)

</div>

</div>

NOTE:
SAY:
- Secure Shell is a modern standard for remote terminal access.
- SSH was created by [Tatu Ylonen](https://ylonen.org/) in 1995 as a successor to telnet (port 23) and FTP (port 21), which were heavily used at the time.
- SSH uses password authentication to establish a terminal-only connection to a computer running the SSH service
- Requires port 22 to be open on the "server"
- Many applications such as WinSCP and VSCode can "piggyback" SSH by using it as a background means of transferring data

---

<!-- .element class="split-screen-with-title" -->
# RDP

<div>

<div>

- Microsoft Remote Desktop Protocol (RDP) is built into Microsoft Windows.
  - Uses TCP port 3389
  - Not known for greatest security, but within a LAN like our home it's fine
  - Can be used by macOS if installed separately
- XRDP is software installed to Ubuntu Linux Desktop to act as RDP server
  - Allows Windows/macOS clients to connect via RDP

</div>

<div>

![Image](/ops-102-guide/curriculum/class-07/slides/assets/10_0.png)

</div>

</div>

NOTE:
SAY:
- Remote Desktop Protocol (RDP) is a proprietary protocol developed by Microsoft that enables remote access to a Windows-based computer over a network connection.
  - RDP is built into Microsoft Windows operating systems, allowing users to establish remote desktop sessions and control a remote computer as if they were physically present at the machine.
- RDP utilizes TCP port 3389 for communication between the client and the remote desktop server.
- While RDP is convenient for remote access within a LAN such as a home network, it is important to note that RDP has had some security vulnerabilities in the past.
  - It is advisable to apply security best practices, such as using strong passwords and keeping the operating system and RDP client up to date with security patches.
- For macOS users, RDP support is not natively built into the operating system.
  - However, Microsoft provides an official Remote Desktop client for macOS that can be installed separately to enable RDP functionality.
  - Today's lab will walk you through how to do that.

- On Ubuntu Linux desktop systems, you can install and configure software called XRDP, which acts as an RDP server.
  - XRDP allows Windows and macOS clients to connect to the Ubuntu Linux system using the RDP protocol.
  - This enables remote desktop access from Windows or macOS machines to the Ubuntu Linux desktop environment.
- XRDP provides an alternative solution for Linux users who need to access their Ubuntu desktop remotely using RDP, allowing them to leverage the familiar RDP client software available on Windows and macOS platforms.

---

<!-- .element class="split-screen-with-title" -->
# SCP

<div>

<div>

- Secure Copy Protocol (SCP) lets you transfer files from one computer to another
  - Normally, you'd use the command line to do so
  - Today we'll be using a graphical user interface (GUI) mostly for ease of use in form of WinSCP or Cyberduck
- Setup SSH server first on lab kit PC
- Run WinSCP on your personal computer

</div>

<div>

![Image](/ops-102-guide/curriculum/class-07/slides/assets/11_0.png)

</div>

</div>

NOTE:
SAY:
- SCP, or Secure Copy Protocol, is a network protocol that enables secure file transfer between computers.
  - It provides a secure alternative to traditional file transfer protocols like FTP (File Transfer Protocol).
  - SCP uses Secure Shell (SSH) for authentication and encryption, ensuring the confidentiality and integrity of data during transit.
- To transfer files using SCP, you typically use the command line.
  - However, for the purpose of simplicity and ease, we will be using a graphical user interface (GUI) called WinSCP or Cyberduck.
    - WinSCP is a popular open-source SCP client for Windows that provides a user-friendly interface for file transfer operations.
      - It supports both SCP and SFTP (SSH File Transfer Protocol).
    - Cyberduck is also an open-source file transfer client with a user-friendly interface.
      - It allows you to easily connect to remote servers, manage files using drag-and-drop, and edit files directly on the server.
- Before using SCP with WinSCP, you need to set up an SSH server on the lab kit PC, which will act as the destination for file transfer.
  - This involves installing and configuring an SSH server software, such as OpenSSH, on the lab kit PC.
  - Ensure that the SSH server is properly configured with appropriate security settings.
    - think "firewall"
- Once the SSH server is set up, you can run WinSCP or Cyberduck on your personal computer.
- After launching WinSCP or Cyberduck, you will be prompted to enter the connection details for the lab kit PC.
  - This includes the IP address and/or hostname of the lab kit PC, the SSH port (port 22), and the login credentials (username and password) for accessing the SSH server.
- Once the connection is established, WinSCP/Cyberduck will display a split-screen interface.
  - The left pane represents the file system of your personal computer, while the right pane represents the file system of the lab kit PC.
  - You can navigate through the directories and select files to transfer between the two systems.
  - Simply drag and drop the files.
- During the file transfer, WinSCP/Cyberduck encrypts the data using SSH, ensuring the security of your files.
  - You can monitor the progress of the transfer and view the transfer log for any error messages or additional information.

---

<!-- .element class="main-title" -->
# Demo & Lab


NOTE:
- No need to go through ALL the steps.
- Review the lab tasks and submission instructions in Canvas
- Remind students to complete the reading assignment for next class before the upcoming lecture.

DO:
- Check IP Addresse on Lab Computer
  - `ip a`
- Use the APT package manager to confirm that OpenSSH is installed.
  - `sudo systemctl status ssh.service`
- SSH into your lab computer from your personal computer's CLI
  - `ssh username@192.168.X.XXX`
    - the `username` is your lab's username
  - The first time students connect, they'll need to answer 'yes' to some permission questions.
- Check the username in your personal computer's CLI to validate the SSH connection.
  - `whoami`
- To exit the SSH connection
  - `exit`

- Before students make an RDP connection for the first time, they need to be sure to log out of their lab computer via the monitor and keyboard attached to it.
- Open your RDP client software on your home computer.
- Input the IP address and username of your lab computer into the RDP client on your home computer and establish an RDP connection to your lab computer.
  - PC name: `192.168.X.XXX`
    - Windows users might need to add the username in front of the IP address.
      - `username@192.168.X.XXX`
