<!-- .element class="main-title" -->
# Ops 102: Intro to Computer Operations

Class 09

---

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
- Basic Windows Operations
  - System info lookup
  - Control Panel
  - User management
  - File extensions
  - Disk management
- Open Lab Time

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/2_0.png)

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
# Career Development

<div>

<div>

## Career Coaching
- Professional etiquette
- Professional pitch
- Creating a network
- Job search readiness
- Targeted job search
- Professional materials
- Behavioral interview questions

</div>

<div>

## Certifications
- CompTIA IT Fundamentals
- CompTIA Network+
- CompTIA Security+

</div>

NOTE:

**Career coaching** offers new professionals the necessary tools, knowledge, and confidence to navigate the interview process successfully. It provides a supportive environment for learning, practicing, and refining crucial skills, ultimately increasing their chances of making a positive impression on potential employers and securing their desired job opportunities.

**CompTIA certifications** are important as they validate skills, enhance career opportunities, provide access to quality training, focus on cybersecurity, offer vendor-neutral knowledge, establish professional credibility, and facilitate networking within the IT industry. These certifications are a solid investment for individuals seeking to build a successful career in information technology.

---

<!-- .element class="main-title-and-image" -->
# Linux VS Windows

![Image](/ops-102-guide/curriculum/class-09/slides/assets/6_0.png)

NOTE:
- Windows and Linux are two different operating systems, each with their own set of features, strengths, and weaknesses.
- The choice between Windows and Linux depends on individual preferences, specific use cases, and familiarity with the operating system.
- Windows is widely used in personal and business environments, especially for commercial software compatibility and gaming.
- Linux, on the other hand, is popular among developers, server administrators, and those who prefer open-source solutions and extensive customization options.

---

<!-- .element class="split-screen-with-title" -->
# Side by Side

<div>

<div>

# Windows

![Image](/ops-102-guide/curriculum/class-09/slides/assets/5_0.png)

</div>

<div>

# Linux

![Image](/ops-102-guide/curriculum/class-09/slides/assets/5_1.png)

</div>

NOTE:
The differences in file structure, especially the location of the user home directory and user files, will vary between Windows and Linux operating systems.

### Windows File Structure:

**Drive Letters:**
   - In Windows, storage devices such as hard drives and SSDs are assigned letters (C:, D:, etc.). Each drive functions as its own file system hierarchy.

**User Home Directory:**
   - In Windows, the user's home directory is typically located in `C:\Users\<username>`. For example, if the username is "john," the home directory would be `C:\Users\john`.

**Path Separator:**
   - Windows uses backslashes (\) as the path separator in file paths. For example, `C:\Users\john\Documents\file.txt`.

### Linux File Structure (Based on the Filesystem Hierarchy Standard - FHS):

**Root Directory:**
   - Linux has a single root directory, denoted as `/`. Everything in Linux is organized under this root directory.

**Mount Points:**
   - Storage devices in Linux are mounted as directories under the root directory. For example, the main hard drive might be mounted at `/`, and additional storage devices could be mounted at locations like `/mnt/data` or `/media/usb`.

**User Home Directory:**
   - In Linux, the user's home directory is typically located in `/home/<username>`. For example, if the username is "john," the home directory would be `/home/john`.

**Path Separator:**
   - Linux uses forward slashes (/) as the path separator. For example, `/home/john/Documents/file.txt`.

### Differences and Implications:

**Drive Letters vs. Mount Points:**
   - Windows uses drive letters to represent different storage devices, while Linux uses mount points. This means that in Linux, all devices are accessed under a unified directory structure, simplifying file management and navigation.

**User Home Directory Location:**
   - The location of the user home directory differs between Windows and Linux. This variance can affect how applications are configured, especially if they rely on specific paths.

**Path Separators:**
   - Windows and Linux use different symbols (\ in Windows and / in Linux) as path separators. This difference can impact the compatibility of scripts and software that rely on specific path conventions.

---

<!-- .element class="main-title-and-image" -->
# Side by Side

![Image](/ops-102-guide/curriculum/class-09/slides/assets/17_0.png)

NOTE:
### LIVE DEMO: Instructor should have a Windows and Linux machine running side by side to show students the differences between the two.

- Key difference to highlight
  - File structure differences
    - Linux (walk students through some of the linux directories)
      - Root (/) = everything on linux is located under this directory
      - /boot = boot files
      - /dev = device files
      - /home = home folders
      - /etc = configuration files
    - Windows (walk students through directories starting at C:\)
  - Show the different drives in Windows vs the drives in Linux under /dev and /mnt
  - For the other points above, show students where they can see these points in effect.


---

<!-- .element class="main-title" -->
# Basic Windows Operations

NOTE:
- Windows operations encompass a diverse range of tools and interfaces tailored for efficient system management.
- The Command Line Interface (CLI) provides a text-based environment for executing commands, allowing users to perform advanced tasks and automate processes.
- The Control Panel serves as a central hub, offering a user-friendly interface to configure system settings, manage user accounts, and customize various aspects of the operating system.
- Additionally, Device Manager provides precise control over hardware components, enabling users to update drivers, troubleshoot device issues, and ensure seamless functionality of peripherals.
- Together, these elements empower users with versatile means to navigate and optimize their Windows experience.

---

<!-- .element class="split-screen-with-title" -->

# Command Prompt

<div>

<div>

- The Windows Command Prompt opens a CLI
  - ipconfig /all
  - ping
- Good for quick, simple operations
- PowerShell is more advanced, greater feature set

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/8_0.png)

</div>

</div>

NOTE:

- **The Windows Command Prompt opens a CLI (Command-Line Interface)**
  - It allows users to interact with the operating system by typing commands.
  - Common commands:
    - `ipconfig /all`: Displays detailed information about all network interfaces, including IP addresses, MAC addresses, and DNS settings.
    - `ping`: Tests network connectivity to a specific IP address or domain by sending ICMP echo request packets.

- **Good for quick, simple operations**
  - The Command Prompt is suitable for performing basic tasks such as file management, network diagnostics, and system configurations.
  - It's lightweight and efficient for executing simple commands and scripts.

- **PowerShell is more advanced, greater feature set**
  - PowerShell is an advanced shell developed by Microsoft, providing a more extensive command-line experience compared to the Command Prompt.
  - It offers a powerful scripting environment, allowing automation of complex tasks and system administration.
  - PowerShell supports object-oriented programming, pipelining, and remote management capabilities.
  - While the Command Prompt is sufficient for basic tasks, PowerShell is the preferred choice for system administrators and power users due to its rich feature set and scripting capabilities.


---

<!-- .element class="split-screen-with-title" -->
# This PC Properties

<div>

<div>

- Start + About pulls up the This PC menu for computer info like name, domain, etc.
  - Device name
  - Processor
  - RAM
  - Edition
- Rename PC
- Join a domain

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/9_0.png)

</div>

</div>

NOTE:

**Start + About pulls up the This PC menu for computer info like name, domain, etc.**
  - The "This PC" menu in Windows provides essential information about the computer.
  - Information displayed includes:
    - **Device name:** The name assigned to the computer for identification on the network.
    - **Processor:** Details about the computer's CPU (Central Processing Unit), such as the model and speed.
    - **RAM:** The amount of random access memory (RAM) installed on the computer.
    - **Edition:** The specific version or edition of Windows installed on the computer.

**Rename PC**
  - Within the This PC menu, users can access settings to rename their computer.
  - Renaming the PC can be useful for personalizing the device's identity on a network or making it easier to recognize.

**Join a domain**
  - Windows allows users to join a domain, which is often used in corporate or networked environments.
  - Joining a domain means integrating the computer into a network controlled by a domain controller. This provides centralized user management, security policies, and other network-related services.
  - By joining a domain, users can access shared resources, authenticate against a central directory, and enjoy other network privileges.

---

<!-- .element class="split-screen-with-title" -->
# DirectX Diagnostic Tool

<div>

<div>

- DirectX Diagnostic Tool provides a detailed breakdown of GPU/display driver/DirectX info
  - Run with command `dxdiag`
  - Driver information for display, sound

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/11_0.png)

</div>

</div>

NOTE:

**DirectX Diagnostic Tool provides a detailed breakdown of GPU/display driver/DirectX info**
  - The DirectX Diagnostic Tool is a Windows utility that provides detailed information about the computer's DirectX components, GPU (Graphics Processing Unit), display driver, and other multimedia hardware and software components.
  - It gives users insights into the system's DirectX version, graphics card, display settings, sound devices, and various system properties related to multimedia performance.

**Run with command `dxdiag`**
  - Users can access the DirectX Diagnostic Tool by typing `dxdiag` in the Windows Run dialog or the Command Prompt.
  - Running this command opens a graphical user interface that displays comprehensive information about the system's DirectX components and multimedia devices.

**Driver information for display, sound**
  - The DirectX Diagnostic Tool provides specific details about the display and sound drivers installed on the computer.
  - For the display, it includes information about the graphics card, driver version, video memory, and current display settings.
  - For sound devices, it lists audio hardware, driver details, and other related information, allowing users to diagnose issues and ensure their multimedia devices are functioning correctly.

---

<!-- .element class="split-screen-with-title" -->
# Control Panel

<div>

<div>

- In Windows, the Control Panel is a central place to configure the system
- Uses:
  - Add/remove users
  - Add/remove programs
  - Add devices and drivers
  - Configure networking
  - Configure security

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/12_0.png)

</div>

</div>

NOTE:

**In Windows, the Control Panel is a central place to configure the system**
  - The Control Panel is a crucial component of the Windows operating system that provides a centralized interface for configuring various settings and managing system preferences.

**Uses:**
  - **Add/Remove Users:**
    - Users can create, modify, or remove user accounts on the computer through the Control Panel. This includes setting up privileges and permissions.
  - **Add/Remove Programs:**
    - Users can install, uninstall, or modify software applications installed on the computer using the Control Panel's Programs and Features section.
  - **Add Devices and Drivers:**
    - The Control Panel allows users to add new hardware devices (like printers, scanners, etc.) and install or update their drivers to ensure proper functionality.
  - **Configure Networking:**
    - Network-related settings such as setting up network connections, configuring IP addresses, managing Wi-Fi networks, and troubleshooting network issues can be done through the Control Panel.
  - **Configure Security:**
    - Users can manage various security settings through the Control Panel, including Windows Firewall configurations, Windows Defender settings, and user account control options.

---

<!-- .element class="split-screen-with-title" -->
# User Accounts

<div>

<div>

- Users are accounts that can login to this Windows PC
- Account types are group designations that specify whether the account has administrator privileges
  - Administrator
  - Standard user

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/13_0.png)

</div>

</div>

NOTE:

**Users are accounts that can log in to this Windows PC**
  - In Windows, user accounts are individual profiles associated with specific users. Each user account has its own settings, files, and permissions, allowing multiple people to use the same computer while maintaining their personalized experience.

**Account types are group designations that specify whether the account has administrator privileges**
  - **Administrator:**
    - An administrator account has full control over the computer. Users with administrator privileges can install software, modify system settings, create and delete other user accounts, and perform various system-wide tasks. This type of account is typically used by system administrators or the computer's owner.
  - **Standard User:**
    - A standard user account has limited privileges. Standard users can use most of the computer's features and install some software, but they cannot make system-wide changes or modify settings that could affect other users. This type of account is suitable for everyday use and provides a level of security by preventing accidental or intentional modifications to critical system files.

---

<!-- .element class="split-screen-with-title" -->
# File Extensions

<div>

<div>

- File extensions are how we tell computers that a file conforms with a data structure standard
  - .ova files are opened by VirtualBox
  - .docx files are opened by word processors
  - .mp3 files are opened by media player software

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/14_0.png)

</div>

</div>

NOTE:

**File extensions are how we tell computers that a file conforms with a data structure standard**
  - File extensions are suffixes attached to filenames to indicate the file format or the type of data stored in the file. They are important for both the operating system and users as they determine which application should be used to open or process the file.

  - **.ova files are opened by VirtualBox:**
    - .ova (Open Virtualization Appliance) files are used for virtual machines. They contain a snapshot of a virtual machine's configuration, including its virtual disk files, and can be opened and imported by virtualization software like Oracle VM VirtualBox.

  - **.docx files are opened by word processors:**
    - .docx files are documents created with Microsoft Word or other word processing software that supports the DOCX format. DOCX is an XML-based file format used for text documents. These files can be opened by various word processing applications, including Microsoft Word, LibreOffice Writer, and Google Docs.

  - **.mp3 files are opened by media player software:**
    - .mp3 files are audio files that use a compression algorithm to reduce the file size without significantly affecting the audio quality. They can be opened and played by various media player software applications, including Windows Media Player, VLC Media Player, iTunes, and many others.

---

<!-- .element class="split-screen-with-title" -->
# Disk Partitioning

<div>

<div>

- In Windows GUI, Disk Management handles disk formatting and partitioning operations.
- From command line, diskpart
  - Create and format disk partitions, which are logical segments of a physical drive

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/15_0.png)

</div>

</div>

NOTE:

**In Windows GUI, Disk Management handles disk formatting and partitioning operations:**
  - Disk Management is a graphical tool in Windows that allows users to manage disks and partitions. It provides an intuitive interface for tasks like creating, deleting, resizing, and formatting partitions on hard drives and other storage devices.

**From the command line, diskpart:**
  - **diskpart** is a command-line disk partitioning utility in Windows. It provides a more advanced and scriptable way to manage disks and partitions.
  - With diskpart, users can:
    - **Create and format disk partitions:** Diskpart allows users to create new partitions on a disk and format them with a specific file system, such as NTFS or FAT32. These partitions are logical segments of a physical drive, allowing for better organization of data and improved system performance.

---

<!-- .element class="split-screen-with-title" -->
# Disk Partitioning

<div>

<div>

- File systems used by Windows OS
  - FAT32
    - Save this for USB flash drives
  - exFAT - Extended File Allocation Table
    - Save this for USB flash drives, attempt at improving FAT32
  - NTFS
    - Windows default for OS and internal drives

</div>

<div>

![Image](/ops-102-guide/curriculum/class-09/slides/assets/16_0.png)

</div>

</div>

NOTE:

**File systems used by Windows OS:**

  - **FAT32:**
    - **Usage:** FAT32 is suitable for USB flash drives, memory cards, and other external storage devices. It is compatible with various operating systems, including Windows, macOS, and Linux.
    - **Note:** FAT32 has a file size limitation of 4 GB, which means individual files larger than 4 GB cannot be stored on a FAT32 partition.

  - **exFAT (Extended File Allocation Table):**
    - **Usage:** Similar to FAT32, exFAT is primarily used for USB flash drives and external storage devices. It is an attempt at improving upon FAT32, providing support for larger file sizes and more efficient storage allocation.
    - **Note:** exFAT is especially useful for devices that need to store files larger than 4 GB, which is the limitation of FAT32.

  - **NTFS (New Technology File System):**
    - **Usage:** NTFS is the default file system for Windows operating systems and is commonly used for internal hard drives and system partitions.
    - **Features:** NTFS supports large file sizes, file and folder permissions, encryption, and other advanced features. It is optimized for performance, reliability, and security, making it the preferred choice for Windows OS and internal drives.

---

<!-- .element class="main-title" -->
# Demo

NOTE:

- Command Line Interface
- Control Panel
- Device Manager

DO: Pull up cmd.exe and demo some basic commands

