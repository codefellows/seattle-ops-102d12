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

---

<!-- .element class="split-screen-with-title" -->
# Agenda

<div>

<div>

- Review
- Network Your Lab Kit PC
- Virtualization vs Containerization
- Command Line Interface
- Demo
- Open Lab Time

</div>

<div>

</div>

![Image](/ops-102-guide/curriculum/class-05/slides/assets/2_0.png)

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
# Network Your Lab PC

<div>

<div>

- You'll have two options to connect your lab kit PC to your home network
  - Ethernet cable (optimal)
    - Category 6 <!-- .element class="medium-text" -->
    - Category 5e <!-- .element class="medium-text" -->
    - Category 5 <!-- .element class="medium-text" -->
  - Wireless USB adapter
- Connect your lab PC today to same LAN as your personal computer

</div>

<div>

![Image](/ops-102-guide/curriculum/class-05/slides/assets/5_2.png)

</div>


</div>

NOTE:
SAY:
- Today your lab PC will need internet connection to complete the lab.
- You'll have two options to connect your lab kit PC to your home network
  - Ethernet cable (optimal)
    - Ethernet cables provide a stable and reliable connection
    - You have three options when it comes to Ethernet cables:
      - Category 6 offers the highest performance and bandwidth capacity.
      - Category 5e provides excellent performance and is used mostly in home networks.
      - Category 5 older standard, still works for basic network connectivity.
  - Wireless USB adapter
    - If an Ethernet connection is not convenient, you can consider using a wireless USB adapter or dongle.
    - A wireless USB adapter allows your lab PC to connect to your home network without the need for physical cables strung throughout your house.
    - Beware, the connection quality may vary depending on the distance from the wireless router and potential interference.
- Be sure to connect your lab PC to same Local Area Network as your personal computer.

---

<!-- .element class="split-screen-with-title" -->
# Virtual Machines

<div>

<div>

- Virtual machines (VMs) abstract away everything below OS
  - A single computer's “horsepower” can fuel multiple VMs
  - Redundancy
  - Portability
    - A VM on VirtualBox = VM on another computer's VirtualBox

</div>

<div>

![Image](/ops-102-guide/curriculum/class-05/slides/assets/7_0.png)

</div>

</div>


NOTE:
SAY:
- Virtual machines (VMs) abstract away everything below OS
  - VMs allow us to abstract or "virtualize" the underlying hardware of a computer.
  - This means that the "horsepower" or computing resources of a single computer can be shared among multiple virtual machines.
    - Each VM will utilize a portion of the host computer's resources, such as CPU, memory, and storage, so be sure to efficiently distribute the utilization of hardware to avoid locking up the host OS.
  - One of the key benefits of virtual machines is their ability to provide redundancy.
    - If one VM fails or crashes, the other VMs running on the same host computer remain unaffected.
  - Portability
    - For instance, a VM created on VirtualBox can be transferred to another computer running VirtualBox.
    - The VM will work seamlessly on the new host, maintaining its configurations and settings.
    - This makes it easier to migrate VMs between different machines or share VMs with colleagues or partners.

---

<!-- .element class="split-screen-with-title" -->
# Hypervisors

<div>

<div>

- Hypervisors are the software applications responsible for virtualization.
  - Type 1
  - Type 2
- Example software
  - vmWare
  - Virtualbox
  - Parallels

</div>

<div>

![Image](/ops-102-guide/curriculum/class-05/slides/assets/8_0.png)
![Image](/ops-102-guide/curriculum/class-05/slides/assets/8_1.png)
![Image](/ops-102-guide/curriculum/class-05/slides/assets/8_2.png)

</div>

</div>


NOTE:
SAY:
- Hypervisors are the software applications responsible for virtualization.
  - They create and manage virtual machines, allowing multiple operating systems to run simultaneously on a single physical computer.
  - There are two types of hypervisors:
    - Type 1
      - Type 1 hypervisors, also known as bare-metal hypervisors, run directly on the host's hardware.
      - They have direct access to the underlying hardware resources, providing high performance and efficiency.
      - Examples of Type 1 hypervisors include VMware ESXi, Microsoft Hyper-V, and Citrix XenServer.
    - Type 2
      - Type 2 hypervisors run as applications within a host operating system.
      - They rely on the host OS for hardware access, which can introduce some performance overhead.
- Example software
  - vmWare
    - Type 2
    - VMware is a leading provider of virtualization software.
    - Their hypervisor solutions, such as VMware ESXi and VMware Workstation, offer  virtualization for enterprise or personal use.
    - VMware's software is known for its advanced features, scalability, and management tools.
  - Virtualbox
    - Type 2
    - VirtualBox is an open-source virtualization software developed by Oracle.
    - VirtualBox is popular with individuals and small businesses due to its user-friendly cross-platform compatibility, and extensive feature set.
  - Parallels
    - Type 2
    - Parallels is a virtualization software designed specifically for macOS.
    - It enables users to run multiple operating systems, including Windows and Linux, seamlessly on their Mac computers.
    - Parallels offers a user-friendly interface, excellent performance, and integration with macOS features.

---

<!-- .element class="split-screen-with-title" -->
# Containers

<div>

<div>

- Containers abstract away everything below the application.
  - Popular tools used today for containerization include Docker and Kubernetes.
  - Not the same as VMs, abstraction takes place at different layer

</div>

<div>

![Image](/ops-102-guide/curriculum/class-05/slides/assets/9_0.png)

</div>

</div>

NOTE:
# Presenter Notes:

SAY:
- You might be wondering why we don't use containers instead.
  - It turns out containerization serves a different purpose than virtualization.
- Containers abstract away everything below the application.
  - They provide an isolated environment for applications to run consistently across different computing environments.
  - Popular tools used today for containerization include Docker and Kubernetes.
    - Docker is a widely adopted platform for creating, deploying, and managing containers.
    - It allows developers to package their applications and dependencies into a container image that can be easily shared and run on any Docker-enabled host.
    - Kubernetes, on the other hand, is a powerful container orchestration platform that automates the deployment, scaling, and management of containerized applications.
  - Containers and virtual machines (VMs) abstract away different layers of the computing stack.
    - Virtual machines abstract away the underlying hardware, allowing multiple operating systems to run on a single physical machine.
    - Containers, on the other hand, abstract away everything below the application layer, providing a consistent and isolated environment.

---

<!-- .element class="image-and-title" -->
# Containers vs VMs


![Image](/ops-102-guide/curriculum/class-05/slides/assets/10_0.png)

NOTE:
SAY:
- Here is a visual depiction of how containerization differs from virtualization.
- At school, we'll only work with virtual machines in VirtualBox.

---

<!-- .element class="title-and-text" -->
# What is the Linux terminal?

- Many versions exist.
- It's an app that you launch on Ubuntu Desktop.
- If Ubuntu Server, is the default way you use the computer.
- Low level interaction with a computer
- GUI desktop is a higher level of abstraction and "hides" the commands

NOTE:
SAY:
- The Linux terminal is a command-line interface that provides direct low-level interaction with a computer running a Linux-based operating system.
- It allows users to execute commands, run scripts, and perform various system operations.
- It's important to note that there are many versions of Linux, and each may have its own terminal implementation.
  - However, the basic principles and functionality remain consistent across different Linux distributions.
- On Ubuntu Desktop, the terminal is an application that you can launch from the graphical user interface (GUI).
  - It provides a text-based interface where you can enter commands and receive textual output.
- If Ubuntu Server, is the default way you use the computer.
  - On Ubuntu Server, the terminal is the default way you interact with the computer.
  - Unlike Ubuntu Desktop, which provides a graphical desktop environment, Ubuntu Server typically operates solely through the command-line interface.
- Low level interaction with a computer
  - The Linux terminal offers a low-level interaction with the computer's operating system.
  - It allows users to directly execute commands, manage files and directories, configure system settings, and perform administrative tasks.
- In contrast to the terminal, a graphical user interface (GUI) desktop environment provides a higher level of abstraction.
  - The GUI desktop "hides" the underlying commands and offers a visual representation of the system, making it more user-friendly for those less familiar with the command line.

---

<!-- .element class="title-and-text" -->
# Why do we need to know Linux terminal?

- Terminal commands are lower level than GUI
- Not all programs have GUI
- Essential for operating Linux
- Enhances efficiency and productivity with automation

NOTE:
SAY:
- Terminal commands provide a lower level of interaction with the operating system compared to graphical user interfaces (GUI).
  - Understanding the terminal allows you to have more direct control and access to system resources and configurations.
- It's important to note that not all programs or applications have a graphical user interface.
  - Many system administration tools, development environments, and powerful utilities are designed to be used solely from the terminal.
  - Without knowledge of the terminal, you may miss out on utilizing these tools and their functionalities.
- The Linux operating system is built upon the Unix philosophy, which emphasizes the command-line interface as a primary means of interacting with the system.
  - To effectively operate and manage a Linux-based system, knowledge of the terminal is crucial.
  - It allows you to perform system administration tasks, configure settings, navigate the file system, and troubleshoot issues efficiently.
- Learning the Linux terminal can significantly enhance your efficiency and productivity.
  - With a wide range of powerful command-line tools and the ability to script repetitive tasks, you can automate workflows and perform complex operations more quickly than through GUI-based interfaces.

---

<!-- .element class="title-and-text" -->
# What is root?

- This is the superuser account of the computer with full clearance.
- The account you use will not be root, by default.
  - Equivalent idea in Windows might be local user vs admin user.
- Older versions of Linux let you start out as root.

NOTE:
SAY:
- In Linux, the root account is the superuser account that has full administrative privileges on the system.
  - It is also referred to as the "root user" or "superuser".
- When you first set up a Linux system, the account you create will not have root privileges by default.
  - This is by design to prevent accidental or unauthorized access to critical system files and operations.
  - To draw a comparison in the Windows operating system, the concept of a root account is similar to the difference between a local user account and an administrator account.
    - By default, the user account in Linux is not granted administrative privileges, similar to a standard user account in Windows.
- It's worth noting that older versions of Linux allowed users to start out as root.
  - However, this practice is generally discouraged now due to security concerns.
  - Starting as root poses a higher risk of accidental system damage or unauthorized access.

---

<!-- .element class="main-title" -->
# Demo and Lab Overview

NOTE:
DO:
- Open a terminal window and point out the prompt (`username@computername`)
  - Explain it is a representation of where you are in the file system
- Show students the following commands:
  - `CTRL+C`
    - is used to break out of a running process or terminate a command.
    - It provides a quick and convenient way to stop a process that might be taking longer than expected.
  - `pwd`
    - stands for "print working directory" and displays the current location in your file system.
    - It is helpful for knowing where you are within the directory structure.
  - `ls`
    - lists the files and directories contained in the current directory.
  - `ls -al`
    - provides more detailed information about the files, such as permissions, ownership, and file sizes.
  - `cd [path]`
    - used to change the directory you are currently in.
    - By specifying the desired path, you can navigate to different directories within the file system.
  - `mkdir [dirname]`
    - used to create a new directory.
    - By specifying a directory name after the command, you can quickly create a new folder.
  - `touch [file name]`
    - is used to create a new file.
    - By specifying a file name after the command, you can create an empty file with that name.
  - `sudo [command]`
    - is used to elevate your command to root or superuser privileges.
    - After entering the sudo command, you will be prompted to enter the root password to execute the command with elevated privileges.
  - `[command name] -[modifier/flag parameter] [target/action parameter]`
    - This is the general syntax for performing an action with a command in the Linux terminal.
    - You can use various commands with specific flags or modifiers to perform different actions on specific targets.

- No need to go through ALL the steps.
- Review the lab tasks and submission instructions in Canvas
- Remind students to complete the reading assignment for next class before the upcoming lecture.
