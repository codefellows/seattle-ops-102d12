<!-- .element class="main-title" -->
# Ops 102: Intro to Computer Operations

Class 02

NOTE:
INSTRUCTOR PREWORK: Instructor will need a 1080p webcam mounted on a flexible arm pointed at the computer case where you are working. Your lab PC will be disassembled and ready to reassemble for today's demonstration.

DO: Point students to the reading assignment. It will help walk them through the lab.

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

</div>

![Image](/ops-102-guide/curriculum/class-01/slides/assets/3_1.png)<!-- .element class="small" -->

NOTE:
SAY:
- Today we will be re-assembling our lab computers. Some might be even upgrading some parts for better performance.
- Remember, throughout this course we'll examine computers at their lowest level of operations.
- We'll work with computer hardware the first two classes, then start working with the bootup sequence before installing a new Ubuntu OS onto our lab computers.
- Then we'll pivot over to networking where we'll set up a SoHo router and remote connection.
- And finally, we introduce virtualization and finish up Windows operations and security settings before we take the 201 Entrance Exam.

---

<!-- .element class="main-title" -->
# Review

What did you learn?

NOTE:
SAY:
- There are 4 skills in language learning: Hearing, speaking, reading, writing and we generally develop them in that order.
- These review sessions are your chance to SPEAK with this new language.
  - Practice using the right words. Let these foreign sounds emanate from YOUR mouth.
  - The names of these esoteric characters matter, and using the wrong one will make a difference to the computer.
- Go around the room and let each student can share a thing learned.
  - Help them use the right words.
  - Document the vocab on the whiteboard.
  - Ask specifically for what was learned by reading about other student’s learning.

---

<!-- .element class="split-screen-with-title" -->
# Review

<div>

<div>

- What is a Computer?
  - Binary & Data
  - Circuits & Logic
  - Inside a Computer
- Lab assignment
  - Disassembly

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/4_0.png)

</div>

</div>


NOTE:
DO:
- Go around the room and ask the students for their experience with the lab.
  - What went well?
  - What went wrong?
  - What was the solution?
- Return to the previous class's README, fill in some review notes and push to the class repo.


---

<!-- .element class="split-screen-with-title" -->
# Build a Computer

<div>

<div>

- Why might we assemble a desktop computer?
  - Enthusiast PC
  - Component swap or upgrade
  - Enterprise with desktops on-site
  - Value - Components more affordable
- What types of desktop computers are there?
  - Gaming
  - CAD Workstation
  - Office
  - Thinclient

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/6_0.png)

</div>

</div>

NOTE:
- Why might we ever need to build or reassemble a desktop PC in an age of laptops? Here are a few scenarios you may encounter:
- Enthusiast PC
  - If you're a PC gamer, you'll want to ensure that you have a solid grasp of desktop assembly, hardware components, performance capabilities, interfaces, and compatibilities.
  - Alternatively, you may need to recommend a higher-performance PC for power users like video editors and CAD workstation users.
  - Often you'll simply need to identify a performance bottleneck for a user you support. A person with 12 large spreadsheets open at any given time may need more RAM, for example.
- Component swap or upgrade
  - Even on laptops, components like RAM and SSD are sometimes replaceable without disassembly (depending on model).
  - Sometimes you can avoid costly purchases by replacing parts versus an entire PC
- Enterprise uses desktops on-site
  - While companies are largely transitioning to laptops, you may still work with a desktop environment where these skills will come in handy.
- Value - Components more affordable
  - Powerful desktop components are still cheaper than their laptop counterparts.
- There's a few different purposes we might use a desktop PC. Think of this class as an opportunity to get to know the components of a computer. Mobile devices still use these components but at a reduced physical footprint!

- What types of desktops are there?
  - Gaming
    - These are designed specifically for gaming enthusiasts and offer high-performance components to handle demanding games.
    - They typically feature powerful processors, dedicated graphics cards, ample RAM, and fast storage options.
  - CAD Workstation
    - Computer-Aided Design
    - These workstations are optimized for running complex design and engineering software.
    - They have powerful processors, high-end graphics cards, and large amounts of RAM to handle intensive tasks like 3D modeling, rendering, and simulations.
  - Office
    - Office desktops are geared towards general productivity tasks in a business or home office environment.
    - They prioritize reliability, efficiency, and affordability.
    - They usually have sufficient processing power for everyday tasks like word processing, spreadsheet management, web browsing, and email.
  - Thinclient
    - Thin clients are lightweight desktop computers that rely on a server or cloud-based infrastructure to perform most computing tasks.
    - They are typically used in business environments where data and applications are stored centrally.
    - Thin clients are cost-effective, energy-efficient, and offer easy manageability since most processing occurs on the server-side.
  - It's worth noting that there are several other specialized desktop categories as well, such as media production workstations, scientific computing systems, and compact form-factor desktops (e.g., mini PCs).

---

<!-- .element class="split-screen-with-title" -->
# Interfaces

<div>

<div>

- Why do computers have various interfaces?
  - Transfer data
- Types
  - User interface
  - Software interface
  - Hardware interface
- In our case we are studying hardware interface.

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/7_0.png)

</div>

</div>

NOTE:
SAY:
- Computer interfaces facilitate the standardized transfer of information.
  - Why, then, are there so many different interfaces?
  - Well, they all serve different purposes, needs, and capabilities of the time in which they were introduced. Remember 56K dialup?
- Let’s identify the types of interfaces depicted in this picture.
  - PS2
    - This interface was commonly used for connecting keyboards and mice to computers.
  - DB25/Parallel/Serial (old printers/peripherals)
    - These interfaces were used for connecting older printers and peripherals to computers.
  - RS232
    - This interface was used for serial communication between computers and devices such as modems and early digital cameras.
  - VGA
    - Video Graphics Array
    - Was a standard interface for connecting monitors to computers, although it has largely been replaced by digital interfaces like HDMI and DisplayPort.
  - USB
    - Universal Serial Bus
    - Is a versatile interface used for connecting a wide range of devices, including storage devices, peripherals, and smartphones.
  - Ethernet
    - Ethernet is used for networking and connecting computers to local area networks (LANs) or the internet.
  - Audio
    - The audio interface allows for connecting speakers, headphones, microphones, and other audio devices to computers.
- An interface is a boundary across which two independent systems meet and act on or communicate with each other. In computer technology, there are several types of interfaces.
  - User interface
    - The user interface includes the keyboard, mouse, menus, and other elements that allow users to interact with the operating system and software applications.
    - Graphical User Interfaces (GUIs) provide visual elements for ease of use.
  - Software interface
    - The software interface comprises the languages, protocols, and codes that applications use to communicate with each other and with the underlying hardware.
    - This includes APIs (Application Programming Interfaces) and other communication protocols.
  - Hardware interface
    - The hardware interface refers to the physical connections, wires, plugs, and sockets that hardware devices use to communicate with each other and with the computer system.
    - These interfaces define how data and signals are transmitted between devices.
- In our case we are studying hardware interface.
  - Be sure to do your own internet research on hardware interfaces.
  - There are lots of great diagrams that highlight all of them.
- Let’s take a look at USB and video interfaces next.

---

<!-- .element class="split-screen-with-title" -->
# USB

<div>

<div>

- Universal Serial Bus (USB) is an industry standard for communications between computers and peripherals due to its versatility and widespread adoption.
- Standards continue evolving to support faster transmission speeds
  - USB 1.1 = 12 Mbps
  - USB 2.0 = 480 Mbps
  - USB 3.0 = 5 Gbps
  - USB 3.1 Gen 2 = 10 Gbps

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/8_0.png)

</div>

</div>

NOTE:
SAY:
- Understanding how data is transferred between devices is crucial for cybersecurity.
- One widely adopted interface for data transfer and power charging is the Universal Serial Bus (USB).
  - It serves as an industry standard for connecting computers and peripherals.
- On the right side of the slide, you can see various examples of USB standards that have evolved over time.
  - These standards have introduced new features and improved data transfer rates.
  - Wikipedia provides a helpful timeline outlining the introduction of each USB standard.
- Let's take a look at the evolution of USB transmission speeds:
  - USB 1.1
    - This was the initial version of USB, offering a maximum data transfer rate of 12 Mbps (megabits per second). It was commonly used for basic peripherals like keyboards and mice.
  - USB 2.0
    - The introduction of USB 2.0 brought a significant leap in speed, offering a maximum transfer rate of 480 Mbps. This increased bandwidth made it suitable for high-speed devices like external hard drives and digital cameras.
  - USB 3.0
    - USB 3.0, also known as SuperSpeed USB, raised the bar even further by providing a maximum transfer rate of 5 Gbps (gigabits per second). This boost in speed enabled faster data transfers and improved performance for devices such as SSDs and high-resolution webcams.
  - USB 3.1 Gen 2
    - Building upon the foundation of USB 3.0, USB 3.1 Gen 2 further enhanced data transfer speeds. It supports a maximum rate of 10 Gbps, allowing for even faster file transfers and smoother operation of advanced peripherals.
- It's essential to note that USB is not only used for data transfer but also for charging devices.
  - Many modern peripherals and mobile devices rely on USB for power delivery, making it a versatile and convenient interface.
- USB is also backward compatible, which means that newer USB devices can still be used with older USB ports, although the speed will be limited to the capabilities of the specific USB version being used.

---

<!-- .element class="split-screen-with-title" -->
# Video Interfaces

<div>

<div>

- VGA
  - an analog interface that carries video signals from the computer to the monitor <!-- .element class="medium-text" -->
- DVI
  - supports both digital and analog video signals, offering better image quality and compatibility with various display devices <!-- .element class="medium-text" -->
- HDMI
  - a digital interface that supports both high-definition video and audio signals, simplifying the connection between devices and eliminating the need for separate audio cables. <!-- .element class="medium-text" -->
- Displayport
  - offers higher bandwidth and supports higher resolutions, including 4K and even 8K displays <!-- .element class="medium-text" -->

</div>

<div>

Video interfaces play a vital role in transferring data from the computer to the monitor, enabling us to see visual content.

![Image](/ops-102-guide/curriculum/class-02/slides/assets/9_0.png)

</div>

</div>

NOTE:
SAY:
- Video interfaces play a vital role in transferring data from the computer to the monitor, enabling us to see visual content.
- Let's explore some common video interfaces that facilitate this data transfer:
  - VGA
    - Video Graphics Array
    - VGA is one of the earliest video interfaces and has been widely used for many years.
    - It is an analog interface that carries video signals from the computer to the monitor.
    - While VGA is still capable of supporting a resolution of 1080p, its analog nature makes it susceptible to signal degradation over longer cable distances.
  - DVI
    - Digital Visual Interface
    - DVI is a digital video interface that replaced VGA in many applications.
    - It supports both digital and analog video signals, offering better image quality and compatibility with various display devices.
    - DVI connectors come in different types, including DVI-D (digital only), DVI-A (analog only), and DVI-I (integrated digital and analog).
    - However, DVI is gradually being phased out in favor of newer interfaces.
  - HDMI
    - High-Definition Multimedia Interface
    - HDMI has become the de facto standard for connecting computers, gaming consoles, Blu-ray players, and other devices to HD displays.
    - It is a digital interface that supports both high-definition video and audio signals, simplifying the connection between devices and eliminating the need for separate audio cables.
    - HDMI has evolved over the years to support higher resolutions, refresh rates, and additional features such as Ethernet connectivity and Audio Return Channel (ARC).
  - DisplayPort
    - DisplayPort is a versatile digital video and audio interface that competes with HDMI.
    - It offers higher bandwidth and supports higher resolutions, including 4K and even 8K displays.
    - DisplayPort also provides features like Multi-Stream Transport (MST) for daisy-chaining multiple monitors and Adaptive Sync for smoother, tear-free gaming experiences.
    - DisplayPort is commonly found on professional monitors and high-end graphics cards.
- Understanding the different video interfaces is crucial for selecting the appropriate cable or adapter when connecting your computer to a monitor or other display devices.
  - It ensures compatibility, optimal image quality, and the ability to take advantage of advanced features offered by newer interfaces.
- As technology continues to advance, it's worth keeping an eye on emerging video interface standards and their capabilities.
  - The market evolves quickly, and staying informed will help you make informed decisions when it comes to video connectivity.

---

<!-- .element class="split-screen-with-title" -->
# Interface Security

<div>

<div>

- Data Protection
  - The security of your data is paramount.
- Malware Threats
  - Portable devices can be carriers of malware.
- Unauthorized Access
  - Hardware interfaces can provide an entry point.
- Data Exfiltration
  - Portable devices can be used to extract sensitive data.

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/10_0.png)

</div>

</div>

NOTE:
SAY:
- First, let me share a story about why computer interfaces, like a USB port can actually be a security threat.

DAVID'S STORY:
- Once upon a time, I had the opportunity to work alongside contracted finance auditors who periodically visited our company's office. These auditors were responsible for reviewing our financial processes and ensuring that appropriate security policies were in place, including those related to data handling. However, an interesting conflict arose during their visits that shed light on the importance of USB security.
- As part of our security policy, the IT department had disabled USB ports from reading flash drives to mitigate the risk of malware entering our systems. USB drives brought in by visitors were scanned for viruses by the IT team before any selective use was allowed. The auditors, who were tasked with assessing our IT security policies, would arrive with their own USB drives to share files during their engagement with the finance team.
- The irony was hard to miss. Here were auditors, responsible for evaluating our IT policies surrounding financial data, bringing in USB drives that hadn't been subjected to our screening process. To make matters more puzzling, they requested that I lift the USB port restrictions on computers for the day, enabling the finance employees to freely exchange files using USB drives.
- This situation highlighted an important takeaway. Portable media devices such as flash drives, portable hard drives, and even cell phones connected via USB can serve as a common attack vector for malware distribution. It becomes crucial to understand the capabilities of computer interfaces and adjust security policies accordingly.

SAY:
- Interface security is a topic that deserves our attention due to the potential risks and consequences associated with it.
- Data Protection
  - Whether it's personal information, confidential business documents, or sensitive files, the security of your data is paramount.
- Malware Threats
  - USB devices can be carriers of malware.
  - When infected USB devices are connected to your computer, malware can spread rapidly, compromising the integrity of your system, stealing sensitive information, or causing damage.
  - Security measures help mitigate the risk of malware infections and protect your devices and data from potential threats.
- Unauthorized Access
  - Hardware interfaces can provide an entry point for unauthorized access to your computer or network.
  - If an attacker gains physical access to your USB device, they may be able to exploit vulnerabilities, execute malicious actions, or extract sensitive information.
  - Implementing security measures helps prevent unauthorized access and safeguards your system against potential intrusions.
- Data Exfiltration
  - Portable devices can be used to extract sensitive data from a computer system.
  - This could be done intentionally by an insider threat or accidentally if something like a USB device is lost or stolen.
  - USB security controls, such as encryption or access controls, help prevent data exfiltration and maintain the confidentiality of your valuable information.

---

<!-- .element class="split-screen-with-title" -->
# Portable Media

<div>

<div>

- USB flash drive
- External hard drive
- CD-ROM or DVD-ROM disk
  - Uses the “.iso” file extension
  - Commonly, used to install software
- Magnetic storage devices (obsolete)
  - Tapes, floppy diskette

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/11_0.png)

</div>

</div>

NOTE:
SAY:
- USB Flash Drive
  - Also known as thumb drives or USB sticks
  - Are portable storage devices that use flash memory to store data.
  - They are compact, lightweight, and offer high storage capacities, making them popular for transferring files between computers and devices.
  - USB flash drives are commonly used for tasks such as backing up important files, sharing documents or media, and booting into operating systems.
- External Hard Drive
  - External hard drives are larger storage devices that connect to computers via USB, Thunderbolt, or other interfaces.
  - They offer larger storage capacities compared to USB flash drives and are commonly used for data backup, archiving large files, or expanding the storage capacity of a computer.
  - External hard drives provide the advantage of being portable while allowing for easy transfer and access to large amounts of data.
- CD-ROM or DVD-ROM Disk
  - CD-ROM and DVD-ROM disks are optical storage media that use lasers to read data stored on them.
  - These disks commonly use the ".iso" file extension, which is a disk image format containing the complete contents of a CD or DVD.
  - CD-ROM or DVD-ROM disks are often used for software installation, distribution of multimedia content, or sharing large files that can be burned onto these disks.
- Magnetic Storage Devices (Obsolete)
  - In the past, magnetic storage devices like tapes and floppy diskettes were widely used for data storage and transfer. However, they are now considered obsolete due to limited storage capacity and technological advancements.
  - Magnetic tape drives were used for data backup, large-scale data storage, and archival purposes.
  - Floppy diskettes, often known as floppy disks, were small, removable storage devices primarily used for transferring and storing small files.

---

<!-- .element class="split-screen-with-title" -->
# Analog VS Digital

<div>

<div>

- Both Analog and Digital signals use electricity to transmit information.
- Analog Signal: Information translated into electric pulses of different amplitudes. Examples: VGA interface, old stereo receivers
- Digital Signal: Information is in binary format (0 and 1) and there are only two amplitudes. Examples: HDMI, modern stereo decks

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/12_0.png)

![Image](/ops-102-guide/curriculum/class-02/slides/assets/12_1.png)

</div>

</div>

NOTE:
SAY:
- When it comes to transmitting information via electrical signals, both analog and digital methods serve the same purpose. However, they employ different techniques to achieve this goal, making them distinct from each other.
- Analog is the older sibling of the family and has largely been surpassed by the newer and more popular digital approach.
- Analog signals modify wave amplitudes to represent information, while digital signals use binary values of ones and zeroes for communication. For instance, video interfaces like VGA rely on analog signals, whereas HDMI utilizes digital signals.
- Despite the differences, both analog and digital signals are capable of supporting high-definition resolutions, such as 1080p.
- Analog signals translate information into electric pulses with varying amplitudes, allowing for a continuous range of values. Examples of analog interfaces include VGA interfaces and older stereo receivers.
- Digital signals, on the other hand, encode information in binary format, employing only two amplitude levels: 0 and 1. This discrete nature enables precise data representation. Examples of digital interfaces include HDMI and modern stereo decks.

---

<!-- .element class="split-screen-with-title" -->
# Memory
### How do computers store data?

<div>

<div>

- Volatile memory vanishes upon shutdown or reboot
  - CMOS
  - Random access memory (RAM)
  - Cache memory
- Non-volatile memory persists upon shutdown or reboot
  - HDD, SSD
  - Read only memory (ROM)
  - Optical
  - Magnetic (Floppy, Tapes)

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/13_0.png)

</div>

</div>

NOTE:
SAY:
- Computers not only process data, but they also rely on memory to store data, either temporarily or for the long term.
- It's important to recognize that memory vulnerabilities can be exploited by security attacks, making memory security a critical consideration.
  - One notable vulnerability is buffer overflow, which occurs when data exceeds the bounds of a memory buffer, allowing unauthorized commands to be executed.
  - This exploit poses significant security risks and can result in various detrimental consequences.
  - Think of video game speedrunners going "out of bounds" to understand the potential threats associated with this type of attack.
- Volatile memory, as the name suggests, is temporary in nature.
  - It stores data while the computer is powered on but is lost upon reboot or shutdown.
  - Security forensics teams prioritize the recovery of volatile data as it can provide crucial insights into system activities and potential security breaches.
  - Examples of volatile memory include CMOS, RAM, and cache-based memory.
- Caches are allocated memory spaces used for temporary storage to expedite processing.
  - Web browsers, for instance, utilize web page content caches to accelerate loading times.
  - It's important to note that cache memory can also be exploited in cyber attacks, as demonstrated by the Spectre/Meltdown vulnerabilities that abused CPU memory caches.
- Non-volatile memory, in contrast, retains data even during power loss or system reboots.
  - Examples of non-volatile memory include hard disks, ROM (Read-Only Memory), optical media like CDs and DVDs, and magnetic media such as floppy disks.

---

<!-- .element class="split-screen-with-title" -->
# Hard Drives

<div>

<div>

- Platter drive (HDD) use optical disk media for memory storage
  - Older, slower
  - Cheapter (gap is closing)
- Solid state drive (SSD) use flash technology to store memory
  - Much faster than HDD
- M.2 drive are the fastest and most costly
  - Slightly faster than SSD (often not appreciable difference)
  - Most expensive

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/14_0.png)

</div>

</div>

NOTE:
SAY:
- When it comes to storage drives, there are different types to consider, each with its own characteristics and trade-offs.
- Platter Drive
  - HDD, or Hard Disk Drive, is an older and more traditional type of storage drive.
  - While HDDs are slower compared to other drive types, they have historically been more affordable, making them a popular choice for mass storage needs.
  - HDDs use spinning platters and magnetic heads to read and write data. The data is stored on these platters, allowing for large storage capacities at relatively lower costs
- Solid State Drive
  - SSDs, or Solid State Drives, are newer storage drives that have gained significant popularity in recent years.
  - SSDs offer significantly faster data access and transfer speeds compared to HDDs, resulting in improved overall system performance.
  - SSDs utilize flash memory technology, which provides faster read and write operations, making them ideal for applications that require quick data access, such as operating system boot times, loading applications, and file transfers.
- M.2 Drive
  - M.2 drives are a specific form factor of storage drives that are becoming increasingly popular in modern systems.
  - M.2 drives typically utilize solid state memory technology like SSDs, providing similar performance benefits.
  - While M.2 drives may offer a slight performance advantage over traditional SSDs, the difference is often not appreciable in everyday use cases.
  - It's worth noting that M.2 drives are generally more expensive compared to traditional HDDs or standard SSDs due to their compact form factor and high-speed capabilities.

---

<!-- .element class="split-screen-with-title" -->
# Data and Power Interfaces

<div>

<div>

- Data interfaces
  - Serial ATA (SATA) is now most common hard disk power and data interface standard <!-- .element class="medium-text" -->
- Power interfaces
  - Serial ATA (SATA) power is the 15-pin SATA power connector <!-- .element class="medium-text" -->
  - Molex is the older 4-pin power connector <!-- .element class="medium-text" -->
- Power supply unit (PSU) converts Alternating Current (AC) to usable Direct Current (DC)
  - Newer units are modular <!-- .element class="medium-text" -->
  - Motherboard, component power <!-- .element class="medium-text" -->

</div>

<div>

![Image](/ops-102-guide/curriculum/class-02/slides/assets/15_1.png)

</div>

</div>


NOTE:
SAY:
- When it comes to computer interfaces, USB is commonly used for connecting external devices.
- However, there are various data and power interfaces utilized within the computer itself.
- Let's explore the different data and power interfaces commonly found in computer systems:
  - Data Interfaces:
    - Serial ATA (SATA)
      - SATA interfaces are used for data transfer between the motherboard and internal storage devices like HDDs and SSDs. They provide reliable and high-speed data transmission.
    - Power Interfaces
      - SATA power connectors are used to deliver power to SATA-based storage devices. They are commonly seen in HDDs and SSDs.
      - Molex connectors are older power connectors used for various components in the computer system, such as fans or older optical drives.
    - Power Supply Unit (PSU):
      - Think of the PSU as a "transformer" that steps down the voltage from the incoming power source and converts it from Alternating Current (AC) to usable Direct Current (DC) for the computer's components.
        - It ensures a stable and regulated power supply to all components.
      - The PSU connects to the motherboard and provides power to all the components, including the CPU, GPU, drives, and peripherals.
      - Newer PSU models often feature modular designs, allowing for easier cable management and customization of power connections.
- For demanding computer setups such as gaming or CAD workstations, it's important to have a PSU with a higher power capability to supply adequate power to handle the system's requirements.

---

<!-- .element class="split-screen-with-title" -->
# Build a Computer - Steps

<div>

<div>

- Setup a PC case and power supply
- Install the CPU and heatsink + fan to motherboard
- Install memory components (RAM, SSD/HDD)

</div>

<div>

- Install all other components (GPU, Cooling, Sound Card, etc.)
- Attach power cabling from PSU to component
- Attach data cabling

</div>

</div>

NOTE:
SAY:
- Setup a PC case and power supply:
   - Begin by selecting a suitable PC case that meets your requirements for size, aesthetics, and cooling capabilities. Open the case and position it in a well-ventilated area.
   - Install the power supply unit (PSU) into the designated area of the case, ensuring a secure fit. Connect the necessary power cables to the PSU for future component connections.
- Install the CPU and heatsink + fan to motherboard:
   - Carefully align the CPU with the corresponding socket on the motherboard, ensuring correct orientation. Gently place the CPU into the socket and secure it according to the motherboard's instructions.
   - Apply thermal paste to the top of the CPU to ensure optimal heat transfer. Attach the heatsink and fan assembly to the CPU socket, making sure it is properly secured.
- Install memory components (RAM, SSD/HDD):
   - Insert the RAM modules into the appropriate slots on the motherboard, aligning the notches and applying gentle pressure until they click into place.
   - For SSDs or HDDs, locate the drive bays in the PC case. Slide the SSD or HDD into the respective bay, securing it using screws or the case's tool-less installation mechanism.
- Install all other components (GPU, Cooling, Sound Card, etc.):
   - Install the graphics card (GPU) into the designated PCIe slot on the motherboard, securing it with screws if necessary. Connect any required power cables to the GPU.
   - If additional cooling components, such as case fans or liquid cooling systems, are desired, install them according to the manufacturer's instructions.
   - If a sound card or other expansion cards are necessary, insert them into the appropriate PCIe slots on the motherboard.
- Attach power cabling from PSU to components:
   - Connect the necessary power cables from the PSU to the motherboard, ensuring all power connectors are securely attached.
   - Connect power cables from the PSU to the graphics card and other components that require power.
- Attach data cabling:
   - Connect the SATA data cables from the motherboard to the SSDs or HDDs, ensuring a secure connection.
   - If using an optical drive or other peripherals, connect their respective data cables to the appropriate connectors on the motherboard.

---

<!-- .element class="main-title" -->
# Demo and Lab Overview

NOTE:
DO:
- No need to go through ALL the steps.
- Review the lab tasks and submission instructions in Canvas
- Remind students to complete the reading assignment for next class before the upcoming lecture.
