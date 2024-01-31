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

- Review
- 201 Entrance Exam Review
- Feedback Survey
- Take the 201 Entrance Exam

</div>

<div>

![Image](/ops-102-guide/curriculum/class-10/slides/assets/2_0.png)

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
## About the 201 Entrance Exam

<div>

<div>

- This is an individual test meaning that you may NOT collaborate with others.
- 15 questions total
- A score of 80% or higher is required to pass the exam.
  - If you fail the exam, contact your instructor.

</div>

<div>

- As you prepare to take this test, think of it as a quiz covering all of the Ops 102 topics.
- You are not expected to solve these challenges just by looking over the choices. You ​are expected to use your Ops tools and problem-solving skills to find the answers.
- There is no time limit in which it must be completed. Just finish taking the exam before the end of today.

</div>

</div>

NOTE:
SAY:
- This is an individual test meaning that you may NOT collaborate with others.
- 15 questions total
- A score of 80% or higher is required to pass the exam.
  - If you fail the exam, contact your instructor, who will meet with you to review areas you should approach differently. Your instructor may grant you a single retake at their discretion.
- As you prepare to take this test, think of it as a quiz covering all of the Ops 102 topics.
- You are not expected to solve these challenges just by looking over the choices. You ​are expected to use your Ops tools and problem-solving skills to find the answers.
- There is no time limit in which it must be completed. Just finish taking the exam before the end of today.

---

<!-- .element class="title-and-text" -->
## When we installed Ubuntu onto our lab computers, what steps did we take next, in order to boot from the SSD/HDD? Why?

<div>

- Remove the USB flash drive and reboot the PC  <!-- .element: class="fragment" data-fragment-index="1" -->
- Because we programmed BIOS to boot from the USB first and then if a USB was not detected, to boot from the hard drive.  <!-- .element: class="fragment" data-fragment-index="2" -->

</div>

NOTE:
SAY:
-

---

<!-- .element class="title-and-text" -->
## What is RAM?

<div>

- RAM stands for Random Access Memory.  <!-- .element: class="fragment" data-fragment-index="1" -->
- It is a type of computer memory that is used for temporary storage of data that is actively being used or processed by a computer's operating system, applications, and processes. <!-- .element: class="fragment" data-fragment-index="2" -->
- RAM provides fast access to data while the computer is running, but the data is erased when the computer is shut down. <!-- .element: class="fragment" data-fragment-index="3" -->
- RAM stores data in volatile memory. <!-- .element: class="fragment" data-fragment-index="4" -->

## What is volatile memory? <!-- .element: class="fragment" data-fragment-index="5" -->
- Volatile memory is a type of computer memory that loses its stored data when the power is turned off. <!-- .element: class="fragment" data-fragment-index="6" -->
- Non-volatile memory, such as hard drives, is used for long-term data storage.  <!-- .element: class="fragment" data-fragment-index="7" -->

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## What does it mean to "partition and format" a storage device?

<div>

- Partitioning is the process of dividing a physical storage device, such as a hard disk drive (HDD) or solid-state drive (SSD), into separate sections called partitions. <!-- .element: class="fragment" data-fragment-index="1" -->
  - Each partition behaves as a separate unit with its own file system, acting as if it were an independent drive. <!-- .element: class="fragment" data-fragment-index="2" -->
  - Partitioning allows you to create multiple logical drives within a single physical device. <!-- .element: class="fragment" data-fragment-index="3" -->
- Formatting establishes a file system on a partition to determine how data is stored and accessed. <!-- .element: class="fragment" data-fragment-index="4" -->
  - It creates the necessary structures on the partition to store files, directories, and metadata. <!-- .element: class="fragment" data-fragment-index="5" -->
- Partitioning and formatting will permanently erase any existing data on a drive. <!-- .element: class="fragment" data-fragment-index="6" -->

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## What is a hardware interface?

<div>

- It is the physical connection between two or more hardware components. <!-- .element: class="fragment" data-fragment-index="1" -->
- Peripheral interfaces connect peripheral devices, such as keyboards, mice, printers, scanners, and external storage devices, to a computer or another host device. <!-- .element: class="fragment" data-fragment-index="2" -->
  - Common peripheral interfaces include USB, Thunderbolt, HDMI, and Ethernet. <!-- .element: class="medium-text" -->
- Storage interfaces facilitate the connection between a computer and storage devices like hard disk drives, solid-state drives, or optical drives. <!-- .element: class="fragment" data-fragment-index="3" -->
  - Examples of storage interfaces include SATA (Serial ATA), SCSI (Small Computer System Interface), and NVMe (Non-Volatile Memory Express). <!-- .element: class="medium-text" -->
- Display interfaces transmit video and audio signals from a computer or media player to a display device, such as a monitor or a television. <!-- .element: class="fragment" data-fragment-index="4" -->
  - Well-known display interfaces include VGA (Video Graphics Array), DVI (Digital Visual Interface), HDMI, DisplayPort, and Thunderbolt. <!-- .element: class="medium-text" -->
- Expansion card interfaces allow additional cards or modules to be connected to a computer's motherboard to expand its functionality. <!-- .element: class="fragment" data-fragment-index="5" -->
  - Examples include PCI (Peripheral Component Interconnect), PCI Express, and AGP (Accelerated Graphics Port). <!-- .element: class="medium-text" -->

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `diff` <!-- .element: class="code" class="dark" -->

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- The diff command is a command-line utility available in Unix-like operating systems, including Linux and macOS.
- It is used to compare the contents of two files or directories and identify the differences between them.
- psuedocode: `diff file1 file2` <!-- .element: class="code" class="dark" -->

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `ip a` <!-- .element: class="code" class="dark" -->

- This command is used in Linux-based operating systems to display detailed information about the network interfaces including: <!-- .element: class="fragment" data-fragment-index="1" -->
    - interface names
    - link states
    - MAC addresses
    - IP addresses (both IPv4 and IPv6)
    - broadcast addresses
    - subnet masks
    - network scopes
    - network interface flags
- Used for managing and troubleshooting network configurations. <!-- .element: class="fragment" data-fragment-index="2" -->

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `systeminfo` <!-- .element: class="code" class="dark" -->

- This command is used in Windows to retrieve detailed information about a computer's hardware and software configuration. <!-- .element: class="fragment" data-fragment-index="1" -->
  - It provides information such as the operating system version, system manufacturer, processor details, installed memory (RAM), and more.
  - This command is often used for system troubleshooting or to gather system information for technical support.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `ipconfig /all` <!-- .element: class="code" class="dark" -->

- This command is used in Windows to display the configuration details of all network interfaces on a computer. <!-- .element: class="fragment" data-fragment-index="1" -->
  - It provides information about the IP address, subnet mask, default gateway, DNS servers, and other network settings.
  - This command is helpful for diagnosing network connectivity issues and verifying network configuration.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `ping` <!-- .element: class="code" class="dark" -->

- This command is used to test network connectivity between two devices. <!-- .element: class="fragment" data-fragment-index="1" -->
  - By sending ICMP (Internet Control Message Protocol) echo request packets to a specific IP address or hostname, it measures the round-trip time and checks for packet loss.
  - The ping command is widely used to troubleshoot network connectivity problems and determine the responsiveness of a network device.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `tracert` <!-- .element: class="code" class="dark" -->

- short for "traceroute" <!-- .element: class="fragment" data-fragment-index="1" -->
  - This command is used to trace the route that packets take from a source device to a destination device or host on a network.
  - It displays the IP addresses of intermediate routers or hops along the path, along with the round-trip time for each hop.
  - This command helps diagnose network latency and identifies network issues or bottlenecks.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `regedit` <!-- .element: class="code" class="dark" -->

- This command opens the Windows Registry Editor, a powerful tool for viewing, modifying, and managing the Windows Registry. <!-- .element: class="fragment" data-fragment-index="1" -->
  - The Windows Registry stores configuration settings and options for the operating system, hardware, and installed applications.
  - `regedit` allows you to navigate through the registry's hierarchical structure and make changes to registry keys and values.
  - Caution must be exercised when using `regedit` since modifying the registry incorrectly can cause system instability or even render the system inoperable.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `msconfig` <!-- .element: class="code" class="dark" -->

- This command opens the System Configuration utility in Windows. <!-- .element: class="fragment" data-fragment-index="1" -->
  - This utility allows you to manage startup programs, services, boot options, and system settings.
  - It provides a convenient way to troubleshoot startup issues, manage system resources, and make configuration changes without directly editing system files.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## Describe the command `dxdiag` <!-- .element: class="code" class="dark" -->

- This command opens the DirectX Diagnostic Tool on Windows. <!-- .element: class="fragment" data-fragment-index="1" -->
  - It provides detailed information about a computer's hardware, drivers, and DirectX components.
  - The tool is useful for diagnosing graphics and audio issues, verifying driver versions, and checking DirectX compatibility.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
## What is the difference between Red Hat Enterprise Linux and Kali Linux 20.04?

<div>

- Red Hat Enterprise Linux is a commercial Linux distribution primarily used for enterprise deployments, while Kali Linux 20.04 is a specialized distribution focused on penetration testing and cybersecurity. <!-- .element: class="fragment" data-fragment-index="1" -->
  - Target Audience and Purpose  <!-- .element: class="fragment" data-fragment-index="2" -->
    - Red Hat Enterprise Linux is a commercial Linux distribution aimed at business environments and primarly used for servers and data centers. <!-- .element class="small-text" -->
    - Kali Linux is a specialized Linux distribution focused on penetration testing, ethical hacking, and cybersecurity.<!-- .element class="small-text" -->
  - Package Management <!-- .element: class="fragment" data-fragment-index="3" -->
    - Red Hat Enterprise Linux uses the Red Hat Package Manager (RPM) for package management.<!-- .element class="small-text" -->
    - Kali Linux, based on Debian, uses the Advanced Packaging Tool (APT) for package management.<!-- .element class="small-text" -->
  - Support and Updates  <!-- .element: class="fragment" data-fragment-index="4" -->
    - Red Hat Enterprise Linu is a commercial distribution that provides long-term support, security updates, and maintenance through subscription-based services.<!-- .element class="small-text" -->
    - Kali Linux is a community-driven distribution.<!-- .element class="small-text" -->

</div>

NOTE:
SAY:
- What is the difference between Red Hat Enterprise Linux and Kali Linux 20.04?
  - Red Hat Enterprise Linux is a commercial Linux distribution primarily used for enterprise deployments, while Kali Linux 20.04 is a specialized distribution focused on penetration testing and cybersecurity.
  - Target Audience and Purpose:
    - Red Hat Enterprise Linux is a commercial Linux distribution primarily aimed at enterprise and business environments.
      - It focuses on stability, reliability, and long-term support. RHEL is commonly used for server deployments, data centers, and cloud infrastructure.
    - Kali Linux is a specialized Linux distribution focused on penetration testing, ethical hacking, and cybersecurity.
      - It is designed for security professionals, researchers, and enthusiasts who require powerful tools for testing and evaluating system vulnerabilities.
  - Package Management:
    - Red Hat Enterprise Linux uses the Red Hat Package Manager (RPM) for package management.
      - It utilizes the YUM (Yellowdog Updater, Modified) package manager or the more recent DNF (Dandified YUM) package manager for package installation, updates, and dependency management.
    - Kali Linux, based on Debian, uses the Advanced Packaging Tool (APT) for package management.
      - It utilizes the `apt-get` or `apt` commands to install, update, and manage software packages.
  - Support and Updates:
    - Red Hat Enterprise Linu is a commercial distribution that provides long-term support, security updates, and maintenance through subscription-based services.
      - Red Hat offers different support levels, including technical support and access to patches and updates.
    - Kali Linux is a community-driven distribution.
      - While it does not offer official support to the same extent as RHEL, it benefits from the wider Debian community for updates and security patches.
      - Kali Linux releases are updated regularly, and community support is available through forums and online communities.

---

<!-- .element class="title-and-text" -->
## Where is the IP address located at in this `ip a`<!-- .element: class="code" class="dark" --> output?

```
2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    link/ether 08:00:27:98:2d:57 brd ff:ff:ff:ff:ff:ff
    inet 10.0.2.15/24 brd 10.0.2.255 scope global dynamic noprefixroute enp0s3
       valid_lft 73604sec preferred_lft 73604sec
    inet6 fe80::6562:7962:8fba:b9f5/64 scope link noprefixroute
       valid_lft forever preferred_lft forever
```

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- Located in the line that starts with "inet", the IP address is listed as `10.0.2.15`.
  - The `/24` after the IP address represents the subnet mask, indicating that it is a Class C IP address with a subnet mask of `255.255.255.0`.
  - The inet6 line indicates the IPv6 link-local address associated with the interface.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# What is the SCP command used for?

<div><!-- .element: class="fragment" data-fragment-index="1" -->

- stands for "Secure Copy"
- It is used for securely transferring files between a local host and a remote host over a network.
- It utilizes the SSH protocol for authentication and encryption, providing a secure method for file transfer.
- pseudocode: `scp source_file destination_file`<!-- .element: class="code" class="dark" -->
  - The `source_file`<!-- .element: class="code" class="dark" --> represents the file or directory you want to copy, and the `destination_file`<!-- .element: class="code" class="dark" --> specifies the target location where you want to place the file.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe the different parts of a file:

<div>

- File Name <!-- .element: class="fragment" data-fragment-index="1" -->
  - The file name is the primary identifier for a file and provides a unique name to distinguish one file from another within a directory. The file name is often followed by a file extension, which indicates the file type or format. <!-- .element: class="fragment" data-fragment-index="2" -->
- File Extension <!-- .element: class="fragment" data-fragment-index="3" -->
  - The file extension is a set of characters that appear after the file name and a period (dot). It denotes the file's format or type. File extensions can help both users and operating systems understand how to handle and interpret the file. <!-- .element: class="fragment" data-fragment-index="4" -->
    - Examples of file extensions include `.txt`<!-- .element: class="code" class="dark" --> for text files, `.jpg`<!-- .element: class="code" class="dark" --> for image files, `.mp3`<!-- .element: class="code" class="dark" --> for audio files, and `.docx`<!-- .element: class="code" class="dark" --> for Microsoft Word documents.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe the different parts of a file:

<div>

- File Size <!-- .element: class="fragment" data-fragment-index="1" -->
  - The file size indicates the amount of storage space the file occupies on a disk or storage medium. It is typically measured in bytes, kilobytes (KB), megabytes (MB), gigabytes (GB), or larger units. The file size helps determine the space required to store or transfer the file. <!-- .element: class="fragment" data-fragment-index="2" -->
- File Content <!-- .element: class="fragment" data-fragment-index="3" -->
  - The file content is the actual data stored within the file. It can be text, binary code, images, audio, video, or any other type of data. The content depends on the file's format and purpose. <!-- .element: class="fragment" data-fragment-index="4" -->
      - For example, a text file contains human-readable text, an image file contains image data, and an executable file contains machine code instructions.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe the different parts of a file:

<div>

- File Metadata <!-- .element: class="fragment" data-fragment-index="1" -->
  - File metadata refers to additional information associated with the file. This metadata includes attributes such as creation date, modification date, access permissions, file ownership, file type, and other properties. The metadata provides important details about the file and helps the operating system manage and organize files efficiently. <!-- .element: class="fragment" data-fragment-index="2" -->
- File Path <!-- .element: class="fragment" data-fragment-index="3" -->
  - The file path specifies the location of the file within a file system. It represents the directory hierarchy or folder structure leading to the file. A file path includes the names of the parent directories, separated by a delimiter, like a forwardslash or backslash, and ends with the file name. <!-- .element: class="fragment" data-fragment-index="4" -->
      - For example, in the path `/home/user/docs/file.txt,`<!-- .element: class="code" class="dark" --> `/home/user/docs`<!-- .element: class="code" class="dark" --> is the directory path, and `file.txt`<!-- .element: class="code" class="dark" --> is the file name.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this Windows tool: Windows Device Manager

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- The Windows Device Manager is a management tool that provides detailed information about the hardware devices installed on a Windows computer.
- It allows users to view and control the hardware components, drivers, and their properties.
- You can access Device Manager by right-clicking on the "Start" button and selecting "Device Manager" or by searching for "Device Manager" in the Windows search bar.
- Within Device Manager, you can update drivers, enable or disable devices, view device status, manage device resources, and troubleshoot hardware issues.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this Windows tool: System Information

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- System Information, also known as "msinfo32" (short for Microsoft System Information), is a utility in Windows that provides comprehensive information about the computer's hardware, software, and system components.
- It displays details about the operating system version, hardware specifications, installed software and drivers, network configuration, system resources, and more.
- You can access System Information by pressing the `Windows key + R`<!-- .element: class="code" class="dark" --> to open the Run dialog box, typing `msinfo32,`<!-- .element: class="code" class="dark" --> and pressing `Enter`<!-- .element: class="code" class="dark" -->.
- It's a useful tool for diagnosing system issues, gathering system information for support purposes, and monitoring hardware and software configurations.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this Windows tool: Control Panel

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- The Control Panel is a centralized configuration and management tool in Windows that allows users to customize and control various system settings and features.
- It provides a GUI to access and modify settings related to user accounts, security, network configuration, hardware and devices, power options, appearance and personalization, and more.
- The Control Panel can be accessed by searching for "Control Panel" in the Windows search bar or via the Start menu.
  - However, note that in newer versions of Windows, certain settings and features have been migrated to the modern Settings app.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this Windows tool: Registry Editor

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- The Registry Editor is a Windows tool that enables users to view and modify the Windows Registry, which is a hierarchical database that stores configuration settings, options, and information about the operating system, hardware, installed software, and user preferences.
- It allows users to manually edit registry keys and values, import or export registry files, search for specific entries, and make advanced system changes.
- To access the Registry Editor, you can press the `Windows key + R` to open the Run dialog box, type `regedit,` and press `Enter`.
- The Registry Editor provides access to a critical system component and should be used with caution as incorrect modifications can impact system stability and performance.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# What factors should be considered when optimizing a virtual machine's performance?

<div>

- Optimizing a VM's performance is a balance between resource allocation and avoiding resource overcommitment. <!-- .element: class="fragment" data-fragment-index="1" -->
- Cores <!-- .element: class="fragment" data-fragment-index="2" -->
  - By allocating 2 cores from the host's 4-core CPU to the VM, you provide it with sufficient processing power to handle its workload effectively. This configuration allows the VM to utilize multiple cores for parallel processing, which can significantly enhance performance for tasks that can be parallelized. <!-- .element: class="medium-text" -->
- RAM <!-- .element: class="fragment" data-fragment-index="4" -->
  - Assigning 8GB of the host's 16GB RAM to the VM ensures that it has enough memory to handle its applications and processes efficiently. With 8GB of RAM, the VM can comfortably run resource-intensive applications. <!-- .element: class="medium-text" -->
- Storage <!-- .element: class="fragment" data-fragment-index="6" -->
  - Assigning 500GB of the host's 1TB HDD storage to the VM provides ample disk space for the VM's operating system, applications, and data storage. This allocation ensures that the VM has enough room to store and access its files without running into space limitations, which can cause performance degradation or operational issues. <!-- .element: class="medium-text" -->

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this wireless encryption method: WEP

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- Wired Equivalent Privacy
- WEP was the first wireless encryption protocol introduced. However, it is now considered weak and easily compromised. It uses a shared key authentication and RC4 encryption algorithm.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this wireless encryption method: WPA

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- Wi-Fi Protected Access
- WPA is an improved encryption protocol designed to address the vulnerabilities of WEP. It uses a stronger encryption algorithm called TKIP (Temporal Key Integrity Protocol) and provides better security through dynamic encryption key generation.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this wireless encryption method: WPA2

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- Wi-Fi Protected Access 2
- WPA2 is the current industry-standard wireless encryption protocol. It offers stronger security than WPA by utilizing the AES (Advanced Encryption Standard) algorithm for encryption. It supports two modes: WPA2-Personal (pre-shared key) for home and small office networks, and WPA2-Enterprise (802.1X authentication) for larger organizations.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this wireless encryption method: WPA3

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- Wi-Fi Protected Access 3
- WPA3 is the latest generation of wireless encryption. It enhances security by introducing several new features, including Simultaneous Authentication of Equals (SAE) for stronger password-based authentication and encryption, as well as encryption of individual data packets to protect data privacy even if the pre-shared key is compromised.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Describe this wireless encryption method: EAP

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- Extensible Authentication Protocol
- EAP is not an encryption method itself, but an authentication framework used in enterprise-level wireless networks. It enables different authentication methods, such as EAP-TLS (Transport Layer Security) and EAP-PEAP (Protected EAP), to secure wireless communications by verifying the identities of connecting devices.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# What is the purpose of a patch panel?

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- A patch panel is a device used in networking and telecommunications infrastructure to organize and manage the connections between incoming and outgoing network cables.
- The purpose of a patch panel is to provide a structured and convenient way to manage network connections.
- It typically consists of multiple ports or jacks, usually in the form of RJ-45 connectors for Ethernet networks.
- These ports are arranged in a panel, usually in a rack-mountable form factor.
- Patch panels are commonly used in data centers and server rooms where there is a need for efficient cable management and easy network connectivity.

</div>

NOTE:
SAY:

---

<!-- .element class="title-and-text" -->
# Does the cord color and ordering matter to the ethernet termination standard?

<div> <!-- .element: class="fragment" data-fragment-index="1" -->

- Yes, the color and ordering of the wires within an Ethernet cable matter for proper termination.
- Adhering to the specified color-coding and arrangement, as defined by standards like T568-A or T568-B, ensures compatibility and successful communication between network devices.
- It is important to use the same wiring standard on both ends of the cable for a reliable connection.

</div>

NOTE:
SAY:

---

<!-- .element class="title-text" -->
# Join us for Ops 201: Foundations of Computer Operations

<div>

- Deliver remote IT service and support
- Deploy an EC2 and Lightsail instance on AWS cloud
- Apply a troubleshooting methodology
- Utilize imaging, backup and recovery tools
- Practice the Windows and Linux CLI
- And way more!
- Final Project Presentation

</div>

---

<!-- .element class="main-title" -->
# Feedback Survey

NOTE:
SAY:
- Your feedback is a real gift.
- Our role as instructors is to guide the you through the curriculum, give you direct feedback, and support you through the technical and emotional journey that this intense experience inspires.
- Students invest a lot of time and money to take our classes and our instruction is very interactive which just means that we rely on your feedback to shape your experience here at Code Fellows.
- At the end of every week during your program, we will ask for your feedback in the form of a Canvas assignment.
  - This assignment is EASY points so please DO NOT skip it!
- The first question in the survey asks if you would recommend this course to a friend.
  - Let me set the scene for you, if you knew someone who was looking to change careers into the tech industry, would you recommend our course?
  - Then tell us WHY or why NOT!
- Be honest in your feedback and try to come from a place of factual observation vs emotionally motivated. Your feedback is what makes the course better for both you and future students.

