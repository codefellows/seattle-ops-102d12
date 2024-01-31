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
- Today we'll take a crash course in computer networking, then configure the lab router that came bundled in your kit.
- Networking is unto itself a vast and complex field of IT, but by end of today you'll be able to configure and deploy a basic SoHo network and gain more insight into the protocols that drive it.

---

<!-- .element class="split-screen-with-title" -->
# Agenda

<div>

<div>

- Review
- Computer Networking
- SoHo Network Configuration
  - IP Addresses
  - Routers
- Lab

</div>

<div>

![Image](/ops-102-guide/curriculum/class-06/slides/assets/2_0.png)

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

<!-- .element class="main-title" -->
# Computer Networking

NOTE:
DAVID'S STORY:
- Running out of IPs
SAY:
- On one of the networks I was overseeing several years back, we had just added a warehouse to an existing network, so lots of new computers and phones were about to be added.
- We counted the computers and figured our network capacity was big enough, so we proceeded.
- A week later, one user's computer fell of the network. When we rebooted it, it would be fine for the day.
- Then the next day, a different computer would lose network.
- This kept happening for several days until we reviewed the network and found out that personal cell phones had been hogging what we call “IP addresses.”
- Only then did we realize; the computers were competing for virtual real estate with cell phones!
- This is called “DHCP Starvation”
- there were not enough IP addresses to go around, so all the computers were squabbling over them!
- Imagine that, your computer getting in an argument with another one.
- Sound preposterous? Welcome to networking!!

---

<!-- .element class="split-screen-with-title" -->
# Our Lab Plan

<div>

<div>

- Deploy a small office/home office (SOHO) router.
- Configure it to broadcast a secure wireless network.
- You'll need:
  - Lab router
  - Power adapter
  - Ethernet cables
  - A web browser for accessing the router's configuration interface.

</div>

<div>

![Our Lab Topology](/ops-102-guide/curriculum/class-06/slides/assets/new-lab-topology.png)

</div>

</div>

NOTE:
SAY:
- The objective of today's lab is to understand the process of deploying a SOHO router and configuring it to broadcast a secure wireless network.
- By the end of this lab, you should be able to set up a secure wireless network for a small office or home environment.

---

<!-- .element class="title-and-text" -->
# Network Configuration

- `ipconfig` for Windows
- `ifconfig -a` for Linux/Mac (older)
  - `ip addr show` (newer for Linux)
- These commands provide valuable information about network interfaces and IP configurations.
- Look for these in the output:
  - MAC address
  - IP address
  - Subnet Mask
  - Gateway address

NOTE:
SAY:
- These commands are essential for obtaining information about network interfaces and IP configurations.
- In Windows, the command to use is `ipconfig` to retrieve IP configuration details.
- In Linux/Mac, the older command is `ifconfig -a,`
- However, Linux has a newer command which is `ip addr show` and this is the one we will be using today on our lab machines.
- In the output of the `ip addr show` command, you can find the following information:
  - MAC address
    - The MAC address is displayed under the `link/ether` field for each network interface.
    - It is a unique identifier assigned to the network interface card (NIC).
  - IP address
    - The IP address is shown under the `inet` field.
    - It indicates the assigned IP address for each network interface.
    - The IP address is often followed by a subnet mask and network prefix length.
  - Subnet Mask
    - The subnet mask is presented along with the IP address under the `inet` field.
    - It indicates the network portion of the IP address and helps determine which part of the IP address represents the network and host.
  - Gateway address
    - The gateway address, also known as the default gateway, is not explicitly displayed in the `ip addr show` output.
    - It is part of the routing configuration.
    - To find the gateway address, you can use the `ip route` command or check the routing table with `ip route show` command.

---

<!-- .element class="main-title" -->
# SoHo Network Configuration

NOTE:
DAVID'S STORY:
- Faulty router
- For one of the clients I supported, the router would constantly go down for no apparent reason (at least once a week).
- Along with it would go an entire network of computers, and a LOT of user complaints.
- Rebooting it always fixed the immediate outage.
- When I finally replaced the router, I noticed it was heavily customized and you could not simply install a replacement and walk away.
- Router configurations can be very specific to the networks they service.
- After a few hours of copy-pasting, the network was back to its original, operational self again.

---

<!-- .element class="split-screen-with-title" -->
#  IP Addresses

<div>

<div>

- Internet Protocol (IP) Addresses serve as unique addresses, allowing devices to send and receive data over the internet.
  - Identification <!-- .element class="medium-text" -->
  - Routing <!-- .element class="medium-text" -->
- A subnetwork or "sub-net" is a network inside a network
  - Like a block of homes within a neighborhood. <!-- .element class="medium-text" -->
  - IP address and the “subnet mask” decide which computers can see each other. <!-- .element class="medium-text" -->
- IP addresses and subnet masks are written with “dotted quad” notation
  - example: `172.16.254.3` <!-- .element class="medium-text" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-06/slides/assets/11_0.png)

</div>

</div>

NOTE:
SAY:
- Internet Protocol (IP) addresses are numerical identifiers assigned to devices connected to a network that uses the Internet Protocol for communication.
- They serve as unique addresses, allowing devices to send and receive data over the internet.
- IP addresses are composed of a series of binary digits, typically represented in human-readable form as a series of four numbers separated by periods.
  - This format is known as "dotted decimal notation."
  - Each number in the address represents an 8-bit segment, ranging from 0 to 255.
- IP addresses serve two primary purposes:
  - Identification
    - IP addresses uniquely identify devices on a network, enabling communication between them. Every device, whether it's a computer, smartphone, or internet-connected device, is assigned an IP address.
  - Routing
    - IP addresses facilitate the routing of data packets across networks. Routers and other networking devices use IP addresses to determine the most efficient path for data transmission, ensuring that information reaches its intended destination.
- A "sub-net" is a network within a network, allowing further segmentation and organization.
  - It can be compared to a block of homes within a neighborhood, where each block represents a subnet.
- IP addresses, along with the subnet mask, determine which computers can communicate with each other within a subnet.
  - The subnet mask specifies the network portion and host portion of the IP address, enabling devices to determine if they are part of the same subnet.
- IP addresses and subnet masks are written in a format called "dotted quad" notation.
  - In this notation, each segment of the IP address or subnet mask is separated by periods (dots).
  - For example, an IP address could be represented as `172.16.254.3`.

---

<!-- .element class="split-screen-with-title" -->
# Routers

<div>

<div>

> “Routers guide and direct network data, using packets that contain various kinds of data—such as files, communications, and simple transmissions like web interactions.”
Cisco

</div>

<div>

![Image](/ops-102-guide/curriculum/class-06/slides/assets/12_0.png)

</div>

</div>

NOTE:
SAY:
- This is a quote directly from Cisco that defines routers.
- Router play a crucial role in directing and forwarding network traffic, ensuring that data reaches its intended destination.

---

<!-- .element class="split-screen-with-title" -->
# Routers

<div>

<div>

- MAC Address is the media access control address uniquely assigned to a network interface by a manufacturer.
- Routers use MAC addresses within data packets to determine where to forward that data in a local network.
- A valid MAC address would consist of six pairs of hexadecimal digits in this format:

`00:00:00:00:00:00`

</div>

<div>

![Image](/ops-102-guide/curriculum/class-06/slides/assets/13_0.png)

</div>

</div>

NOTE:
SAY:
- Routers and MAC addresses are both essential components in the process of data transmission within a network.
- A MAC (Media Access Control) address is a unique identifier assigned to a network interface card (NIC) or network adapter.
  - It is a hardware address that is permanently assigned during the manufacturing process.
- When a router receives a package, it examines the destination MAC address within it to determine if the data packet is intended for its own network segment or another network segment.
  - If the destination MAC address belongs to a device within the same local network, the router forwards it directly to that device.
- A valid MAC address would consist of six pairs of hexadecimal digits in this format: `00:00:00:00:00:00`

---

<!-- .element class="main-title" -->
# Demo - SoHo Router

NOTE:
SAY:
- You need to know the IP address of the router to access its web portal.
  - The default IP address is often mentioned in the router's documentation or can be found on the router itself.
  - Common default addresses are `192.168.0.1` or `192.168.1.1`.
- How do I find my router's IP address in Ubuntu?
  - `ip route | grep default | awk '{print $3}'`
    - `ip route` displays the routing table, which includes information about network routes.
    - `grep` default filters the output to show only the line containing the default route.
    - `awk '{print $3}'` extracts and prints the third field, which represents the IP address of the default gateway (router).

DO:
-  Launch a web browser on your Linux computer.
-  In the address bar of the web browser, type the router's IP address obtained in the previous step and press Enter.

SAY:
- The web browser will display the router's login page.
  - Enter the router's default username and password to log in.
  - Common defaults are "admin" for both the username and password, but this can vary depending on the router brand and model.
  - Once you change the login credentials, you can use the new customized username and password.
- Once successfully logged in, you will be directed to the router's configuration interface.
  - Here, you can access various settings and options to configure the router according to your needs.
  - The interface may have different sections and menus depending on the router manufacturer.

DO:
- Show students the SOHO router web portal.
- Give them a general feel for where things are located and talk about the vocabulary they see here, and test for understanding of terms like “DHCP” and “IP Address.”
  - DHCP
    - DHCP is a network protocol used to dynamically assign IP addresses and other network configuration settings to devices on a network.
    - It simplifies the process of network configuration by automating the assignment of IP addresses, subnet masks, default gateways, and DNS server addresses.
    - With DHCP, devices can join a network and obtain necessary network settings automatically, eliminating the need for manual configuration.
    - DHCP servers manage and distribute IP addresses from a predefined range called a DHCP pool.
  - IP Address
    - An IP (Internet Protocol) address is a unique numerical identifier assigned to each device connected to a network.
    - It enables devices to communicate and identify each other on an IP-based network, such as the internet or a local network.
    - IP addresses can be either IPv4 (32-bit) or IPv6 (128-bit). IPv4 addresses are written in the format "x.x.x.x" (e.g., 192.168.0.1), while IPv6 addresses are written in a hexadecimal format with colons separating segments (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
    - IP addresses are essential for routing data packets across networks, allowing devices to send and receive data to and from specific destinations.
    - They are typically assigned statically (manually configured) or dynamically (automatically assigned via DHCP) depending on the network's requirements.
