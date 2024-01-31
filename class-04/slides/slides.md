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

</div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/3_1.png)<!-- .element class="small" -->

NOTE:

---

<!-- .element class="main-title" -->
# Review

- What did you learn?
- What did you struggle with?
- What blockers did you encounter?
- What fun or cool solutions did you come up with?

NOTE:
- Startup Sequence and BIOS
  - Prowler Boot Sector Virus
  - Startup Sequence
    - ROM, RAM, POST, CMOS
  - BIOS
DO: Go around the class and let students talk about what they learned previous class.

---

<!-- .element class="main-title" -->
# Operating Systems

NOTE:
SAY:
- In this class we'll be working with the latest release of Windows 10 Operating System (OS).
- Don't be surprised, however, if you encounter legacy (older) operating systems during your ops career.
- Many organizations maintain legacy systems for various reasons.
- These reasons might be good or bad.
- An example of a good reason would be when the company operates machinery or special software that only works on Windows XP, for example.

DAVID'S STORY:
- As an IT Manager, I found myself facing a challenging task of managing a diverse array of operating systems. From the ancient relics of Windows 98 and XP to the more recent Windows 7, 8, and 10, my responsibilities were certainly not limited to the cutting-edge technologies. However, I approached this situation as an opportunity to showcase my skills and adaptability.
- While some systems were locked in the grasp of specific operating systems due to vendor requirements, I diligently worked to update as many as possible to the latest Windows 10 version. Embracing the advancements and enhanced security features of the newest OS, I sought to ensure the smooth functioning of the machinery under my care.
- But, as with any job, challenges were abundant. Inevitably, there were instances where I had to delve into the intricacies of legacy systems to provide effective support. This required extensive research and a deep understanding of their unique operations. Undeterred, I eagerly embraced the opportunity to expand my knowledge and conquer these complexities.
- Nevertheless, it was crucial to acknowledge the significance of maintaining up-to-date operating systems from a security standpoint. Beyond the specific cases where updating was infeasible due to business requirements, I recognized the importance of adhering to best security practices. Windows Update, the reliable conduit of security releases from Microsoft, played a central role in safeguarding our systems.
- The peril of operating legacy systems loomed large, with a wealth of known vulnerabilities easily accessible to potential attackers. Thus, I remained vigilant, understanding the urgency of maintaining robust security measures. I strived to implement proactive strategies, such as educating the team about the risks posed by outdated systems and diligently monitoring emerging threats. Through my efforts, I aimed to fortify our defenses and mitigate the potential for exploitation.
- In the face of these challenges, my role as an IT Manager became an ongoing adventure. I embraced the diversity of operating systems and leveraged each opportunity to enhance my skills and protect our technological ecosystem. By striking a delicate balance between preserving legacy systems where necessary and promoting the adoption of the latest OS releases, I sought to ensure the longevity and security of our operations.

---

<!-- .element class="split-screen-with-title" -->
# Operating System

<div>

<div>

- An operating system (OS) is a software program that manages computer hardware and software resources, provides a user interface, and enables the execution of various applications.
- Examples
  - Linux
  - MacOS
  - Windows
  - Android
  - iOS

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/5_0.png)

</div>

</div>

NOTE:
SAY:
- The OS manages hardware and software after being handed controls from the BIOS when its finished booting.
- So we'll often say “boot into Windows.”
- Now that we're booted into the Windows OS, control over hardware and software are in the hands of the OS.
- Here are some other examples of OS; can you name any others?

---

<!-- .element class="split-screen-with-title" -->
# Operating System (OS)

<div>

<div>

- Interface between applications and hardware
- Disk management
- Process management/scheduling
  - Kill process/end task
- Application management
- Memory management
- Device management
- Access control/protection

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/6_0.png)

</div>

</div>

NOTE:
SAY:
- Here's a list of some of the things you can expect the OS to handle.
- The primary functions of an operating system include managing hardware resources (such as the processor, memory, and storage), providing a user interface (such as command-line or graphical), facilitating communication between software and hardware, managing files and directories, and ensuring system security and stability.
- Don't forget even your mobile phones/tablets have OS installed.
  - They may be optimized for touchscreen instead of mouse/keyboard.
- Operating Systems are all around us, even in complex mechanical machinery you'll often see custom apps loaded on top of a familiar OS.

---

<!-- .element class="split-screen-with-title" -->
# Types of OS

<div>

<div>

- Mobile device OS
- Workstation OS
- Server OS
- Embedded OS
- Firmware
- Hypervisor (Type 1)

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/7_0.png)

</div>

</div>

NOTE:
SAY:
- Mobile device OS
  - Mobile device operating systems are designed for smartphones, tablets, and other portable devices.
  - Examples include Android, iOS, and Windows Phone.
  - They are optimized for touchscreens, mobile apps, and connectivity features like mobile data, Wi-Fi, and GPS.
  - Mobile OSs typically provide app stores for downloading and updating applications.
  - They prioritize power efficiency and often include features like battery management and background app restrictions.
- Workstation OS
  - Workstation operating systems are designed for desktop or laptop computers used by individual users.
  - Examples include Windows (e.g., Windows 10), macOS (formerly OS X), and Linux distributions like Ubuntu and Fedora.
  - They offer a range of applications and tools for productivity, multimedia, gaming, and general-purpose computing.
  - Workstation OSs provide a graphical user interface (GUI) and support for various hardware peripherals.
  - They prioritize user productivity, ease of use, and a wide software ecosystem.
- Server OS
  - Server operating systems are designed to run on servers that provide network services, manage resources, and host applications.
  - Examples include Windows Server, Linux distributions like CentOS and Debian, and FreeBSD.
  - They emphasize stability, security, and scalability to handle high workloads and network traffic.
  - Server OSs typically include server-specific features like web servers, database management systems, and virtualization capabilities.
  - They often have command-line interfaces and remote administration tools for managing servers efficiently.
- Embedded OS
  - Embedded operating systems are designed for embedded systems, which are specialized computer systems integrated into other devices or machinery.
  - Examples include Linux-based systems like Embedded Linux, Android (for embedded applications), and real-time operating systems (RTOS) like FreeRTOS.
  - Embedded OSs are lightweight, optimized for specific hardware configurations, and designed for real-time or resource-constrained environments.
  - They are commonly used in devices such as medical equipment, industrial automation systems, smart appliances, and IoT devices.
- Firmware
  - Firmware refers to software that is permanently stored in read-only memory (ROM) or flash memory within a device.
  - It provides low-level control and functionality for specific hardware components or devices.
  - Firmware is often responsible for booting the device, initializing hardware, and providing basic functionality.
  - Examples include BIOS (Basic Input/Output System) in computers and firmware in devices like routers, printers, and game consoles.
  - Firmware updates may be released to fix bugs, enhance performance, or add new features.
- Hypervisor (Type 1)
  - A hypervisor, also known as a virtual machine monitor (VMM), is an operating system or software layer that enables virtualization.
  - Type 1, or bare-metal, hypervisors run directly on the host hardware without the need for a separate OS.
  - Examples of Type 1 hypervisors include VMware ESXi, Microsoft Hyper-V, and Xen.
  - They enable the creation and management of multiple virtual machines (VMs) on a single physical machine.
  - Type 1 hypervisors provide strong isolation between VMs and allow efficient resource allocation and utilization.

---

<!-- .element class="split-screen-with-title" -->
<div>

# OS Market Share

Worldwide, Windows is the most prevalent desktop OS (source)

</div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/8_0.png)

NOTE:
SAY:
- Why don't we study other operating systems in this course?
- We'll work with Ubuntu Linux towards the end of Ops 102, and use Kali Linux in Ops 301 and 401.
- However, the overwhelming market share of endpoint computers goes to Windows by a long margin.
- Again, we're not factoring in servers just yet; these are end user computers for people performing their day-to-day business.
- Globally, Windows has the market at 77%.
- OS X is great to know as well, just keep in mind you are not legally allowed to virtualize macOS on non-Apple hardware.
  - Something you should also be aware of, macOS runs on a Linux command line backend, which we'll start learning in Ops 102 and develop scripting for Bash in Ops 201.
- From a security point of view, if you were writing malware to infect the most computers possible, which OS would you code it for?

---

<!-- .element class="split-screen-with-title" -->
# Origins of Linux

<div>

<div>

- UNIX OS released in 1970 from AT&T Bell Laboratories
  - Widely adopted by academic institutions and businesses
- GNU project launched in 1983 to create a free UNIX-like OS
- Linux created by Linus Torvalds in 1991 and released under GNU public license

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/10_0.png)

</div>

</div>

NOTE:
SAY:
- In 1970, the UNIX operating system was developed at AT&T Bell Laboratories by a team including Dennis Ritchie, Ken Thompson, and others. UNIX became widely adopted by academic institutions and businesses due to its powerful features and portability.
- In 1983, Richard Stallman launched the GNU (GNU's Not UNIX) project with the goal of creating a free and open-source UNIX-like operating system. The project aimed to develop a complete set of software tools, including a kernel, utilities, and libraries.
- In 1991, Linus Torvalds, a Finnish computer science student, created the Linux kernel as a hobby project. Inspired by the Minix operating system and using the GNU tools, Torvalds sought to develop a free and open-source kernel compatible with UNIX-like systems.
- Torvalds combined his Linux kernel with the GNU software to create a complete operating system. This combination of the Linux kernel and GNU software formed the foundation of what is now known as the Linux operating system.
- Linux was released under the GNU General Public License (GPL), a free software license created by Richard Stallman. The GPL ensures that Linux remains open-source, allowing users to access, modify, and distribute the source code.
- Linux gained popularity rapidly due to its free and open nature, stability, and community-driven development. The availability of source code allowed individuals and organizations to contribute to its development, resulting in a robust ecosystem of distributions, applications, and support.
- The Linux community created numerous distributions (distros), each offering different configurations and software choices. Popular distributions include Debian, Ubuntu, Fedora, CentOS, and openSUSE, among many others.
- Linux is now widely used across various domains, including servers, desktops, embedded systems, mobile devices, and supercomputers. It powers a significant portion of the internet, servers, cloud computing platforms, and IoT devices.

---

<!-- .element class="split-screen-with-title" -->
# Why Linux?

<div>

<div>

- Open-source (free)
- Lightweight and less resource-intensive
- Fewer security/privacy issues
- Community support
- Increased software offerings in modern era
- Major market share
- Highly relevant to cybersecurity career
- Related certification CompTIA Linux+

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/11_0.png)

</div>

</div>

NOTE:
SAY:
- Open-source (free)
  - Linux is an open-source operating system, which means it is freely available, and users have the freedom to access, modify, and distribute the source code. This makes Linux a cost-effective option for individuals and organizations.
- Lightweight and less resource-intensive
  - Linux is known for its efficiency and ability to run on older hardware or resource-constrained devices. It is lightweight compared to some other operating systems, allowing it to perform well even on systems with limited resources.
- Fewer security/privacy issues
  - Linux is inherently more secure than some other operating systems due to its design and open-source nature. The large community of developers actively contributes to security enhancements and promptly addresses vulnerabilities. Linux also provides strong privacy features, giving users more control over their data.
- Community support
  - The Linux community is vast and supportive. Users can find help, documentation, forums, and online resources easily. The collaborative nature of the community ensures that Linux users can receive assistance and guidance from experienced users and developers.
- Increased software offerings in the modern era
  - Linux has significantly expanded its software offerings over the years. Many popular applications, development tools, and frameworks are now available for Linux. Additionally, Linux distributions often include package managers, simplifying the installation and management of software.
- Major market share
  - Linux has gained a significant market share, especially in the server and cloud computing domains. Many websites, web servers, and cloud platforms run on Linux. Understanding and being proficient in Linux can provide opportunities for working with these systems and technologies.
- Highly relevant to a cybersecurity career
  - Linux is widely used in the field of cybersecurity. Many security tools, frameworks, and penetration testing distributions are built on Linux. Understanding Linux is valuable for professionals in cybersecurity roles, as it helps in analyzing and securing systems, performing forensic analysis, and working with security tools.
- Related certification CompTIA Linux+
  - The CompTIA Linux+ certification validates foundational knowledge and skills in Linux administration. Obtaining this certification can enhance career prospects in IT, especially in roles related to Linux system administration and support.

---

<!-- .element class="split-screen-with-title" -->
# Why Linux?

<div>

<div>

- Why Ubuntu Linux?
  - Popularity for general computer use
- What are some other common Linux distributions?
  - Red Hat - Great for servers
  - CentOS - Great for Enterprise deployments
  - Kali - Used for offensive security

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/12_0.png) <!-- .element height="175" -->

![Image](/ops-102-guide/curriculum/class-04/slides/assets/12_1.png) <!-- .element height="175" -->

![Image](/ops-102-guide/curriculum/class-04/slides/assets/12_2.png) <!-- .element height="175" -->

</div>

</div>

NOTE:
SAY:
- Why Ubuntu Linux?
  - Ubuntu Linux is a popular choice for general computer use due to its user-friendly interface and widespread adoption.
  - It offers a balance between ease of use and functionality, making it suitable for both beginner and experienced users.
  - Ubuntu has a large and active community, providing extensive support, documentation, and resources for users.
  - The Ubuntu Software Center offers a vast selection of applications, making it easy to find and install software for various needs.
  - Regular releases and long-term support (LTS) versions provide stability, security updates, and a predictable upgrade cycle.
- What are some other common Linux distributions?
  - Red Hat: Red Hat is a popular Linux distribution known for its robustness and stability, making it ideal for server environments. It is widely used in enterprise-level deployments and offers reliable support and long-term maintenance through Red Hat Enterprise Linux (RHEL).
  - CentOS: CentOS is a community-driven distribution derived from the sources of RHEL. It provides a free and open-source alternative to RHEL and is well-suited for enterprise deployments where stability and compatibility with RHEL are essential.
  - Kali: Kali Linux is a specialized distribution focused on offensive security and penetration testing. It comes preloaded with a wide range of tools for vulnerability assessment, network scanning, and digital forensics. It is commonly used by security professionals and ethical hackers.
  - These are just a few examples of the wide variety of Linux distributions available. Each distribution has its own strengths, focus, and target audience, catering to specific needs and preferences.
  - It's worth noting that the Linux ecosystem offers numerous other distributions, including Fedora, Debian, openSUSE, Arch Linux, and many more. Each distribution has its own community, package management system, and philosophies, allowing users to choose the one that best fits their requirements.

---

<!-- .element class="split-screen-with-title" -->
# Linux CLI

<div>

<div>

- Linux OS is known for its powerful command line interface, not its GUI endpoint usability
- Strengths
  - Great for advanced users
  - Software package handling
  - Shell scripting
  - Server administration
  - Shared by MacOS
  - Cyber tools designed for Linux

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/13_0.png)

</div>

</div>

NOTE:
SAY:
- Linux OS is known for its powerful command line interface, not its GUI endpoint usability.
  - Linux is renowned for its powerful command line interface (CLI) that offers extensive control and flexibility over the system.
  - The CLI provides a text-based environment where users can execute commands to perform various tasks, manage files and directories, and configure system settings.
  - While Linux does offer graphical user interface (GUI) options, its strength lies in its CLI, which is preferred by advanced users, system administrators, and developers who value the efficiency and control it provides.
  - The CLI allows for automation, scripting, and remote administration, making it a preferred choice in server environments and for tasks requiring complex and repetitive operations.
- Strengths
  - Great for advanced users: Linux provides a highly customizable and flexible environment that appeals to advanced users who prefer to have fine-grained control over their systems.
  - Software package handling: Linux distributions have robust package management systems, such as apt, yum, and dnf, which simplify the installation, updating, and removal of software packages. This makes software management efficient and straightforward.
  - Shell scripting: Linux's command line interface allows users to write shell scripts, which are sequences of commands that can be executed as a script. Shell scripting is powerful for automating tasks, performing system administration tasks, and creating custom workflows.
  - Server administration: Linux is widely used as a server operating system due to its stability, security, and versatility. It provides a rich set of server administration tools and services, making it a preferred choice for managing web servers, database servers, and other server applications.
  - Shared by macOS: macOS, the operating system used on Apple's Mac computers, is based on a Unix-like foundation (Darwin) that shares commonalities with Linux. This allows users familiar with Linux to leverage their knowledge and skills when working with macOS systems.
  - Cyber tools designed for Linux: The Linux ecosystem has a vast array of cybersecurity tools and frameworks available. Many security professionals and ethical hackers prefer Linux for tasks such as vulnerability assessment, penetration testing, and digital forensics, as it provides a well-supported environment for these activities.

---

<!-- .element class="split-screen-with-title" -->
# OS Performance

<div>

<div>

- Why do operating systems get slower/buggier over time?
  - More apps = More competition for finite system resources (RAM, CPU)
  - More changes made to OS over time
- Why does reinstalling the OS improve user experience?
- What is a “baseline?”

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/14_0.png)

</div>

</div>

NOTE:
SAY:
- Often while supporting various computers, I'd find myself tempted to “wipe” and reinstall the operating system, because the results were always so positive for the end user experience.
  - A fresh Windows installation behaves very predictably.
- Today we'll look at how this is done manually.
- Later on in 201 we'll add more advanced tools to take snapshots in time of computers and restore them.
- So why do computers get slower over time?
  - Well, the OS “ages” as we add more software and make changes to it over time. Reinstalling the OS tends to yield immediate gains in performance because of the “clean slate” effect.
- A “baseline” is a predefined configuration that is known to work as expected. Our baseline for today is the clean installation of Windows 10.

---

<!-- .element class="split-screen-with-title" -->
# Network Topology Diagram

<div>

<div>

- A network topology diagram is a visual representation of a network's devices, connections, and paths.
  - Maps interconnected devices and how they communicate with one another.
- Purposes:
  - Visualize Network Structure
  - Planning and Design
  - Troubleshooting and Maintenance
  - Documentation

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/15_0.png)
[Draw.io](https://app.diagrams.net/) is a good topology tool

</div>

</div>

NOTE:
- A network topology diagram is a visual representation of a network's devices, connections, and paths, allowing you to picture how devices are interconnected and how they communicate with one another.
- Think of this like a map that maps out all the connections in your network.
- A Network topology diagrams serves several purposes:
  - Visualize Network Structure
    - They provide a visual representation of how devices, such as computers, servers, routers, switches, and other network equipment, are interconnected.
  - Planning and Design
    - Network topology diagrams help in planning and designing networks by identifying the components, their relationships, and the overall structure.
  - Troubleshooting and Maintenance
    - They aid in troubleshooting network issues by allowing network administrators to visualize the network and identify potential problem areas.
  - Documentation
    - Topology diagrams act as documentation, capturing the network's current state and facilitating future modifications or expansions.
- Network topology diagrams typically include the following components:
  - Nodes represent devices, such as computers, servers, printers, switches, routers, or firewalls, that are part of the network.
  - Links represent the connections between nodes, which can be wired (Ethernet cables, fiber optic cables) or wireless (Wi-Fi, Bluetooth).
  - Labels provide additional information about nodes, links, or network segments, such as device names, IP addresses, or interface details.
- Network topology diagrams use standardized symbols and icons to represent different network components.
  - Common symbols include squares or rectangles for switches or routers, circles or ovals for computers or servers, and lines or arrows to depict connections.
- They are commonly referred to simply as a "topology" or "topologies".
- Our favorite topology tool is [draw.io](https://app.diagrams.net/).

---

<!-- .element class="title-and-text" -->
# Types of Topologies

<div>

<div>

- Bus Topology
  - Nodes are connected in a linear manner, with each device connected to a single cable or backbone. <!-- .element class="medium-text" -->
- Star Topology
  - Nodes are connected to a central device, such as a switch or hub, forming a star-like structure. <!-- .element class="medium-text" -->
- Ring Topology
  - Nodes are connected in a closed loop, where data flows in one direction around the ring. <!-- .element class="medium-text" -->
- Mesh Topology
  - Nodes are connected to multiple other nodes, creating a redundant and highly interconnected network. <!-- .element class="medium-text" -->
- Hybrid Topology
  - Networks can combine multiple topologies to meet specific requirements. <!-- .element class="medium-text" -->

</div>

</div>

NOTE:
SAY:
- You may come across other types of topologies but these are the most common.

---

<!-- .element class="split-screen-with-title" -->
# Our Lab Plan

<div>

<div>

- Lab kit PC will run Ubuntu Linux Desktop
  - Access from personal computer using Microsoft Remote Desktop Protocol (RDP) over port 3389
  - Also Secure Shell over port 22

</div>

<div>

![Image](/ops-102-guide/curriculum/class-04/slides/assets/15_0.png)

</div>

</div>

NOTE:
- Lab plan
  - Remote into your lab kit PC; private cloud

---

<!-- .element class="main-title" -->
# Demo and Lab Overview

NOTE:
DO:
- No need to go through ALL the steps.
- Review the lab tasks and submission instructions in Canvas
- Remind students to complete the reading assignment for next class before the upcoming lecture.

