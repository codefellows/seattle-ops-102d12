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
- Virtualization
  - Supported operating systems
  - Resource allocation
- Windows OS
  - Versions
  - Editions
- Demo
- Lab

</div>

<div>

![Image](/ops-102-guide/curriculum/class-08/slides/assets/2_0.png)

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
# Virtualizing an OS

<div>

<div>

- Why will we be using VirtualBox?
  - Free
  - Supports .ova file extension import/export without licensing
  - Offers compatibility across different platforms, including Windows, macOS, Linux, and Solaris
  - Allows you to run multiple virtual machines simultaneously on a single host computer.

</div>

<div>

![Image](/ops-102-guide/curriculum/class-08/slides/assets/5_0.png)

</div>

</div>

NOTE:
SAY:
- We will be using VirtualBox for virtualizing an operating system due to several reasons:

- Free
  - VirtualBox is an open-source virtualization platform that is available free of charge.
  - This makes it accessible to users who are looking for a cost-effective solution for virtualization.

- Supports .ova file extension import/export without licensing
  - VirtualBox allows you to import and export virtual machines using the .ova (Open Virtualization Format) file format without any additional licensing requirements.
  - This format provides a convenient way to package and distribute complete images of virtual machines, including the virtual hard drive, configuration settings, and other necessary components.
  - In contrast, some other virtualization software like VMware may have licensing restrictions or limitations when working with .ova files.

- Compatibility
  - VirtualBox is designed to work with different types of computers and supports various operating systems as both host and guest systems.
  - It offers compatibility across different platforms, including Windows, macOS, Linux, and Solaris.
  - This flexibility allows users to create and run virtual machines on different computers, enabling easy migration and sharing of virtual environments.

- Multiple computers on a single host
  - VirtualBox allows you to run multiple virtual machines simultaneously on a single host computer.
  - This feature is useful for scenarios where you need to create and manage multiple virtualized environments on a single physical machine.
  - It enables you to consolidate multiple systems into a single host, saving hardware resources and simplifying the management of virtual machines.

---

<!-- .element class="split-screen-with-title" -->
# Virtualizing an OS

<div>

<div>

- A virtual machine (VM) abstracts away everything below the OS.
  - Only dealing with the OS, networking, apps, etc.
  - A computer inside a computer
  - Multiple computers per host computer
- What is required to virtualize?
  - Intel VT-X or AMD-V capable chipset
  - Host OS that supports the chosen virtualization software
  - Hypervisor software

</div>

<div>

![Image](/ops-102-guide/curriculum/class-08/slides/assets/6_0.png)

</div>

</div>


NOTE:
SAY:
- A virtual machine (VM) acts as an abstraction layer that isolates and encapsulates the underlying hardware and operating system.
  - It provides a virtualized environment where users interact with the operating system, applications, and networking components without having to worry about the underlying hardware details.

  - With a VM, users primarily interact with the OS, applications, and other software components within the virtual environment.
    - They can install and configure software, manage networking settings, and perform other tasks as if they were working on a physical machine.

  - Conceptually, a virtual machine can be thought of as a computer within a computer.
    - It simulates the functionality of a physical computer, including its processor, memory, storage, and network interfaces, while running as a software instance on a host machine.

  - Virtualization technology allows multiple virtual machines to coexist and operate simultaneously on a single host computer.
    - This capability enables the consolidation of multiple systems onto a single physical machine, leading to resource optimization and improved efficiency.

- To virtualize an operating system, several requirements must be met:

  - Hardware Virtualization Support
    - The CPU of the host machine must have hardware virtualization capabilities such as Intel VT-X (Intel Virtualization Technology) or AMD-V (AMD Virtualization).
      - These technologies enable the efficient execution of virtualization instructions, allowing the virtual machine software to run with near-native performance.

  - Compatible Host Operating System
    - The chosen virtualization software requires a host operating system that supports it.
    - Different virtualization software may have specific compatibility requirements, so it's essential to choose software that aligns with the host operating system you intend to use.

  - Hypervisor Software
    - A hypervisor, also known as a virtual machine monitor (VMM), is the software layer responsible for managing and running virtual machines.
    - It creates and manages the virtualized environment, enabling the execution of guest operating systems.
    - The choice of hypervisor software depends on the specific virtualization needs and preferences. Popular examples include VirtualBox, VMware, Hyper-V, and KVM.

---

<!-- .element class="split-screen-with-title" -->
# Virtualizing an OS

<div>

<div>

- What operating systems are we able to virtualize?
  - Linux distributions (GNU public license)
  - Windows non-activated installations from ISO or evaluation editions
  - Not macOS due to Apple's terms of use that forbid virtualizing on non-Apple hardware
  - Not systems to which we don't have legal license (piracy)

</div>

<div>

![Image](/ops-102-guide/curriculum/class-08/slides/assets/7_0.png)

</div>

</div>


NOTE:
SAY:
- When it comes to virtualization, the operating systems that can be virtualized depend on various factors, including licensing agreements and technical compatibility.
- Here are some considerations regarding the virtualization of different operating systems:

- Linux distributions
  - Virtualization of Linux distributions is generally straightforward and widely supported.
  - Many virtualization platforms, including VirtualBox, VMware, and KVM, provide excellent compatibility with various Linux distributions.
  - The GNU General Public License (GPL) allows for the distribution and virtualization of Linux-based operating systems.

- Windows non-activated installations
  - Virtualization of Windows operating systems is possible, even for non-activated installations.
  - You can create virtual machines using ISO files or evaluation editions of Windows.

- macOS
  - Virtualizing macOS on non-Apple hardware is not officially supported due to Apple's terms of use and licensing restrictions.
  - Apple's End User License Agreement (EULA) strictly prohibits the virtualization of macOS on non-Apple hardware.
  - To remain compliant with Apple's terms, virtualization of macOS should only be performed on genuine Apple hardware.

- Legal licensing and piracy
  - It is important to adhere to legal licensing agreements when virtualizing operating systems.
  - Using virtualization to run operating systems for which you do not possess a valid license is considered piracy and is illegal.
  - Virtualization should only be done with legally obtained and licensed copies of operating systems.

---

<!-- .element class="split-screen-with-title" -->
# Virtualizing an OS

<div>

<div>

- What operating systems will we virtualize?
  - Ubuntu 20.10 Desktop
  - Ubuntu 20.10 Server
  - Kali Linux
  - Windows Server 2019
  - Windows 10
  - Windows 7
  - pfSense
    - Not exactly an OS but a router/firewall appliance

</div>

<div>

![Image](/ops-102-guide/curriculum/class-08/slides/assets/8_0.png)

</div>

</div>


NOTE:
SAY:
- Throughout our courses, we will be virtualizing the following operating systems:

- Ubuntu 20.10 Desktop
  - This is a version of the popular Linux-based Ubuntu operating system specifically designed for desktop environments.
  - It provides a user-friendly interface and a wide range of software packages for everyday computing tasks.

- Ubuntu 20.10 Server
  - Ubuntu Server is a version of Ubuntu optimized for server environments.
  - It is a lightweight and powerful operating system designed for running server applications and services.

- Kali Linux
  - Kali Linux is a specialized Linux distribution focused on penetration testing, ethical hacking, and security auditing.
  - It comes with a vast array of tools and utilities used by cybersecurity professionals.

- Windows Server 2019
  - Windows Server 2019 is a server operating system from Microsoft that provides a reliable and scalable platform for running server applications and services.
  - It offers features such as Active Directory, file sharing, virtualization, and more.

- Windows 10
  - Windows 10 is a popular desktop operating system developed by Microsoft.
  - It provides a user-friendly interface and supports a wide range of applications and hardware devices.

- Windows 7
  - Although Windows 7 has reached its end-of-life and is no longer officially supported by Microsoft, it can still be virtualized for specific purposes or compatibility requirements.

- pfSense
  - While not strictly an operating system, pfSense is a free and open-source router/firewall appliance based on FreeBSD.
  - It offers robust network security features, routing capabilities, and firewall functionality.

- These operating systems cover a range of use cases, including general-purpose desktop environments, server deployments, security testing, and network routing/firewalling.

---

<!-- .element class="split-screen-with-title" -->
# Virtualizing an OS

<div>

<div>

- How can I get better performance from virtual machines?
  - Add more RAM is always a good first step
  - Add more CPU speed and cores
  - Consider how you're accessing it
- Fullscreen resolution achievable by installing VirtualBox Guest Additions
  - Devices > Insert Guest Additions CD image
  - Run the installer using ./autorun.sh

</div>

<div>

![Image](/ops-102-guide/curriculum/class-08/slides/assets/9_0.png)

</div>

</div>

NOTE:
SAY:
- To enhance the performance of virtual machines, you can take the following steps:

- Increase RAM
  - Adding more RAM to your virtual machine can significantly improve its performance, especially when running memory-intensive applications.
  - Allocate a higher amount of RAM to the virtual machine within the limits of your host system.

- Increase CPU Resources
  - If your host system has additional CPU cores available, you can allocate more CPU cores to the virtual machine.
  - This can improve the processing power and responsiveness of the virtual machine, particularly when running CPU-intensive tasks.

- Optimize Virtual Machine Settings
  - Adjust the settings of the virtual machine to optimize performance.
  - For example, you can allocate more video memory, enable 3D acceleration, or adjust the virtual disk settings to improve disk performance.

- Consider Access Method
  - The way you access the virtual machine can impact performance.
  - If you are using a graphical interface to access the virtual machine, such as Remote Desktop Protocol (RDP), ensure that your network connection is stable and has sufficient bandwidth for smooth operation.
    - ethernet cord vs WiFi

- To achieve fullscreen resolution in a VirtualBox virtual machine, you can install VirtualBox Guest Additions, which provides additional features and drivers for improved integration between the host and guest systems.

- Here's how you can install it:

1. Start the virtual machine in VirtualBox.
2. From the VirtualBox menu, go to Devices > Insert Guest Additions CD image. This will mount the Guest Additions ISO file to the virtual machine.
3. Within the virtual machine, open a terminal or command prompt.
4. Navigate to the mounted CD image directory. You can usually find it at `/media/cdrom` or a similar location.
5. Run the Guest Additions installer by executing the command `./autorun.sh` (on Linux) or `autorun.exe` (on Windows). This will start the installation process.
6. Follow the on-screen instructions to complete the installation of Guest Additions.
7. Once the installation is finished, restart the virtual machine.

- Google also says that you can run: `sudo apt install virtualbox-guest-additions-iso`

- After installing Guest Additions, you should be able to achieve fullscreen resolution by adjusting the display settings within the virtual machine.
  - This will allow the virtual machine's desktop to match the resolution of your host system, providing a more seamless user experience.

---

<!-- .element class="split-screen-with-title" -->
# Windows OS

<div>

<div>

- Windows adoption business drivers
  - Software and device driver support
  - High compatibility with Microsoft apps
  - Enterprise business environments
  - Gaming apps
  - Active Directory integration for client-server configurations

</div>

<div>

![Image](/ops-102-guide/curriculum/class-08/slides/assets/11_0.png)

</div>

</div>

NOTE:
SAY:
- There are several business drivers that contribute to the adoption of Windows operating systems in different environments.
- Here are some key reasons:

- Software and Device Driver Support
  - Windows enjoys extensive software and device driver support, making it compatible with a wide range of applications and hardware devices.
  - Many software vendors prioritize Windows compatibility, ensuring that their applications run smoothly on Windows-based systems.
  - Similarly, hardware manufacturers often provide Windows drivers, making it easier to use peripherals and devices with Windows.

- High Compatibility with Microsoft Apps
  - Windows operating systems have excellent compatibility with Microsoft's own suite of applications such as Microsoft Office, SharePoint, and Exchange.
  - This makes Windows an ideal choice for businesses heavily reliant on Microsoft software, ensuring seamless integration and optimal performance.

- Enterprise Business Environments
  - Windows is widely adopted in enterprise business environments due to its comprehensive management tools, security features, and support for centralized administration.
  - Windows Server editions offer robust features for server management, Active Directory integration, group policies, and domain-based networks, making it well-suited for large-scale business environments.

- Gaming Apps
  - Windows is the preferred platform for gaming due to its extensive support for gaming libraries, DirectX technology, and a large catalog of game titles developed specifically for Windows.
  - This makes it an attractive choice for businesses or individuals in the gaming industry.

- Active Directory Integration for Client-Server Configurations
  - Windows operating systems seamlessly integrate with Active Directory, which is Microsoft's directory service.
  - Active Directory provides centralized authentication, user management, and policy enforcement, making it beneficial for businesses that rely on client-server configurations and require granular control over user access and permissions.

---

<!-- .element class="split-screen-with-title" -->
# Early Versions of Windows

<div>

<div>

- The original Windows 1.0 OS launched in 1983, a graphical successor to MS-DOS
  - Introduced the Windows GUI <!-- .element class="medium-text" -->
- Windows 10 was released on July 29, 2015.
  - Graphical OS with wide support for drivers and applications <!-- .element class="medium-text" -->
  - Alternatives include Ubuntu Desktop and macOS <!-- .element class="medium-text" -->

</div>

<div>

- Windows 11 was released October 5, 2021
  - modernized user interface, improved productivity features, enhancements for gaming, performance optimizations, better integration with Microsoft services, and improved touch and pen input. <!-- .element class="medium-text" -->

![Image](/ops-102-guide/curriculum/class-08/slides/assets/12_1.png)

</div>

</div>


NOTE:
SAY:
- Windows 1.0
  - Windows 1.0 was launched in 1985 as the first version of the Windows operating system.
  - It was a graphical user interface (GUI) successor to MS-DOS and introduced features like windows, icons, menus, and mouse support.
  - While Windows 1.0 had limited functionality compared to modern versions, it laid the foundation for the future development of Windows.

- Windows 3.1
  - Released in 1992, Windows 3.1 was a significant milestone for Windows as it brought improved performance, enhanced multimedia capabilities, and better support for 32-bit applications.
  - It gained popularity and was widely used during the early 1990s.

- Windows 95
  - Windows 95, released in 1995, introduced a major overhaul to the Windows operating system.
  - It introduced the Start menu, taskbar, and a more user-friendly interface.
  - Windows 95 also provided improved stability, better support for Plug and Play hardware, and long file name support.

- Windows XP
  - Windows XP, released in 2001, became one of the most popular and widely used versions of Windows.
  - It brought a more modern and stable architecture, improved security features, and a revamped user interface.
  - Windows XP was known for its longevity and remained widely used even after the introduction of newer versions.

- Which version was your favorite or least favorite and why?

---

<!-- .element class="split-screen-with-title" -->
# Windows 10 Editions

<div>

<div>

- Graphical OS with wide support for drivers and applications
- Alternatives include Ubuntu and macOS

![Image](/ops-102-guide/curriculum/class-08/slides/assets/13_0.png)

</div>

<div>

- Windows 10 Editions
  - Home
    - Cannot join domains (no client-server) <!-- .element class="medium-text" -->
    - Common off-the-shelf preinstalled <!-- .element class="medium-text" -->
  - Professional
    - Typical version deployed <!-- .element class="medium-text" -->
    - Supports domains <!-- .element class="medium-text" -->
  - Education
    - Designed for educational institutions <!-- .element class="medium-text" -->
    - Tools for managing classrooms <!-- .element class="medium-text" -->
  - Enterprise
    - Catered towards corporations <!-- .element class="medium-text" -->
    - Additional Security, Credential Guard, App Guard <!-- .element class="medium-text" -->

</div>

</div>

NOTE:
SAY:
- Windows 10 is a graphical operating system that offers broad support for drivers and applications.
  - While alternatives like Ubuntu and macOS exist, Windows 10 has its own unique set of editions tailored to different user needs.

- Here are the editions of Windows 10:

- Home
  - Windows 10 Home edition is targeted at home users and offers a wide range of features. It is commonly preinstalled on off-the-shelf computers.
  - However, it does not support joining domains, which means it cannot be used in client-server configurations.

- Professional
  - Windows 10 Professional is the typical version deployed in business environments.
  - It includes all the features of the Home edition and additionally supports joining domains, making it suitable for client-server setups in organizations.

- Education
  - Windows 10 Education edition is designed for educational institutions, such as schools and universities.
  - It includes features that cater to the unique needs of educational environments, including tools for managing classrooms and providing a secure learning environment.

- Enterprise
  - Windows 10 Enterprise edition is primarily aimed at large corporations and organizations.
  - It offers advanced features and enhanced security capabilities like Credential Guard and App Guard provide additional protection against credential theft and malware attacks.

---

<!-- .element class="main-title" -->
# Demo & Lab

NOTE:
- No need to go through ALL the steps.
- Review the lab tasks and submission instructions in Canvas
- Remind students to complete the reading assignment for next class before the upcoming lecture.

SAY:
- You should have already downloaded Windows 10 either directly onto your lab PC or transferred it from your personal computer.

DO:
- Create a new virtual machine:
   - In the VirtualBox main window, click on the "New" button or go to "Machine" and select "New" to start the VM creation wizard.

- Configure the virtual machine:
   - In the VM creation wizard, enter a name for your virtual machine ("Windows 10") and choose the appropriate type and version (Microsoft Windows and Windows 10 64-bit).
   - Click "Next" to proceed.

- Allocate memory (RAM):
  - Choose the amount of memory (RAM) to allocate to the VM. It is recommended to allocate at least 8 GB or more, depending on your system's resources. Adjust the slider or enter the desired amount.
  - How many MB is 8 GB?
    - 8 GB is equal to 8,192 MB.
  - Click "Next" to proceed.

- Create a virtual hard disk:
  - Select the option to create a new virtual hard disk.
  - Choose the hard disk file type (VDI is recommended) and click "Next".

- Choose the hard disk storage:
  - Select the storage type and click "Next". The default option, "Dynamically allocated," is usually suitable for most scenarios.

- Specify the hard disk size:
  - Set the size for the virtual hard disk. Allocate at least 50-100 GB to ensure sufficient space for the Windows 10 installation and any additional software you plan to install.
  - Click "Create" to finish creating the virtual hard disk.

- Configure virtual machine settings:
    - In the VirtualBox main window, select the newly created virtual machine and click on the "Settings" button or go to "Machine" and select "Settings".

- Attach the Windows 10 ISO:
    - In the VM settings window, go to the "Storage" tab.
    - Under "Controller" click on the empty optical drive.
    - In the Attributes section, click on the disk icon and select "Choose/Create Virtual Optical Disk File."
    - Locate and select the Windows 10 ISO file you obtained earlier.
    - Click "OK" to save the changes.

- Set the network adapter to bridge mode.
    - In the VM settings window, go to the "Network" tab.
    - For Adapter 1, set the Attached to value to be "Bridged Adapter"
    - Click "OK" to save the changes.

- Start the virtual machine:
    - In the VirtualBox main window, select the Windows 10 virtual machine and click on the "Start" button.
    - The VM will boot from the Windows 10 ISO and start the installation process.

