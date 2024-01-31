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

<!-- .element class="split-screen-with-title" -->
# Agenda

<div>

<div>

- Review of previous class
  - Share your learning
- Startup Sequence and BIOS
  - Startup Sequence
    - ROM, RAM, POST, CMOS
  - BIOS
  - Demo: BIOS
- Lab Time

</div>

<div>

![Image](/ops-102-guide/curriculum/class-03/slides/assets/2_0.png)

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
- Questions for discussion
  - What happened during POST?
  - What components were listed?
  - Did your computer boot into an operating system?
- Ask specifically for what was learned by reading about other student's learning.

---

<!-- .element class="split-screen-with-title" -->
# Why Startup Sequence?

<div>

<div>

- Why might we need to know the computer startup sequence?
  - Troubleshooting a computer that is not correctly booting
  - Repairing a corrupt master boot record (MBR)
    - MBR holds partition and file system info
    - Boot loader for OS

</div>

<div>

  - Isolated a problem in the startup sequence
  - Accessing BIOS
  - Booting to the correct OS
  - Configuring dual-boot
  - Understanding what's happening behind the scenes

</div>

</div>

NOTE:
SAY:
- Why might we need to know the computer startup sequence?
  - Troubleshooting a computer that is not correctly booting.
    - If a computer is not booting up correctly, knowing the startup sequence can help you to identify the problem and fix it.
  - Repairing a corrupt master boot record (MBR).
    - The MBR is a small piece of code that is stored at the beginning of a hard drive. It contains information about the partitions on the hard drive and the boot loader for the operating system. If the MBR is corrupt, the computer will not be able to boot.
  - Isolating a problem in the startup sequence.
    - If you are having problems with your computer, knowing the startup sequence can help you to isolate the problem to a specific step in the process. This can make it easier to troubleshoot the problem.
  - Accessing BIOS.
    - The BIOS is a small piece of software that is stored on the motherboard of a computer. It is responsible for initializing the hardware and loading the operating system. Knowing the startup sequence can help you to access the BIOS, which can be useful for troubleshooting and configuring your computer.
  - Booting to the correct OS.
    - If you have multiple operating systems installed on your computer, knowing the startup sequence can help you to boot to the correct operating system.
  - Configuring dual-boot.
    - Dual-booting is a way to run two operating systems on the same computer. Knowing the startup sequence can help you to configure your computer to dual-boot.
  - Understanding what's happening behind the scenes.
    - Knowing the startup sequence can help you to understand what is happening behind the scenes when your computer boots up. This can be useful for troubleshooting and for learning more about how computers work.

---

<!-- .element class="split-screen-with-title" -->
# ROM

<div>

<div>

- BIOS originally stored in ROM
  - Newer BIOS use flash memory, less secure
![Image](/ops-102-guide/curriculum/class-03/slides/assets/11_0.png) <!-- .element height="250" -->

</div>

<div>

- ROM is read-only memory.
  - Hard-coded into the motherboard and cannot be altered or deleted
  - Newer devices use flash memory instead of ROM. An example of ROM is the boot sequence of a computer.
![Image](/ops-102-guide/curriculum/class-03/slides/assets/11_1.png) <!-- .element height="250" -->


</div>

</div>

NOTE:
- The BIOS (Basic Input/Output System) is a small piece of software that is stored on the motherboard of a computer.
  - It is responsible for initializing the hardware and loading the operating system.
- The BIOS was originally stored in ROM (read-only memory), which means that it could not be changed or updated.
  - However, newer BIOSes are stored in flash memory, which can be updated. This makes it possible to fix bugs in the BIOS or add new features.
- ROM is a type of memory that is permanently stored on a chip.
  - It cannot be changed or deleted.
  - ROM is often used to store firmware, which is software that controls the hardware of a device.
- Flash memory is a type of memory that can be erased and rewritten.
  - This makes it ideal for storing data that needs to be updated frequently, such as BIOS firmware.
  - Flash memory is also more secure than ROM, because it is not possible to erase it accidentally.

---

<!-- .element class="split-screen-with-title" -->
# Startup

<div>

<div>

- Computer startup
  - The CPU initializes, then fetches instructions from the BIOS, loads into RAM
  - The BIOS starts the monitor and keyboard, system checks
  - The BIOS then starts the boot sequence
    - It will look for the operating system
  - Control transferred to OS

</div>

<div>

![Image](/ops-102-guide/curriculum/class-03/slides/assets/12_0.png)

</div>

</div>

NOTE:
- What happens when a computer turns on?
  - The CPU initializes, then fetches instructions from the BIOS, which is stored in the ROM in older systems (newer systems use flash BIOS). It puts these instructions into RAM for immediate use.
  - Refresh - What is RAM?
    - RAM stands for “random access memory.” RAM is a modular hardware component that is installed onto the motherboard. RAM is like a cache of memory that the computer can use to temporarily store memory it's currently working with for more efficient processing. Examples of RAM-intensive processes include hosting a virtual machine and opening a very large spreadsheet file.
  - The BIOS starts the monitor and keyboard, and does some basic checks to make sure the computer is working properly. For example, it will look for the RAM.
  - The BIOS then starts the boot sequence. It will look for the operating system.
  - If you don't change any of the settings, the BIOS will fetch the operating system from the hard drive and load it into the RAM.
    - This is the part we are going to change in today's lab!
  - The BIOS then transfers control to the operating system.”

---

<!-- .element class="main-title" -->
# BIOS

NOTE:
SAY:
- Next let's take a look at the basic input/output system (BIOS).
- This is a low level computer system that you'll likely never see if you're just an everyday computer user getting work done.
- However, as an ops professional you'll want to familiarize with BIOS from the perspective of computer support and configuration.

DAVID'S STORY:
- When I was a kid, my brother gave me my first PC.
- When I asked him “What's BIOS?” he quickly replied, “Something you should never go into if you don't understand it. Change the wrong setting and you'll break the computer.”
- It turns out this is true; you CAN break a computer if you make a mistake in BIOS.
- For a while I lived in fear of BIOS and never touched it, but once I finally took at look at it, BIOS was a lot less scary than my brother described.
- If you understand computer hardware components and their purpose, there's nothing stopping you from becoming proficient in BIOS configuration.

---

<!-- .element class="split-screen-with-title" -->
# BIOS

<div>

<div>

- Basic Input-Output System (BIOS) is a small piece of software that is stored on the motherboard of a computer and is responsible for initializing the hardware and loading the operating system.

- Look for these in today's lab:
  - Boot modes
    - UEFI
    - Legacy
  - Boot order/priority

</div>

<div>

![Image](/ops-102-guide/curriculum/class-03/slides/assets/14_0.png)

</div>

</div>

NOTE:
SAY:
- BIOS is a small piece of software that is stored on the motherboard of a computer.
  - It is responsible for initializing the hardware and loading the operating system.
  - BIOS is typically stored on a chip on the motherboard.
  - BIOS is written in a low-level language that is specific to the hardware platform.
    - You may see an error during start up if your RAM isn't seated properly, ect.
  - The BIOS can be updated to fix bugs or add new features.
  - The BIOS also loads the operating system into memory.
  - BIOS is responsible for initializing the hardware, such as the CPU, memory, and storage devices.
- The BIOS provides a way to configure the hardware settings of a computer.
  - This can be done by entering the BIOS setup menu, which is usually accessed by pressing a specific key during the boot process.
  - The bootup screen will briefly show you what to press in order to access BIOS.
  - Usually it is keystroke DEL or F2, F10, something like that.
- The BIOS performs a number of tasks when a computer is turned on, including:
  - Power-on self-test (POST)
    - The BIOS runs a series of tests to make sure that the hardware is working properly.
  - Locating the operating system
    - The BIOS searches for the operating system on the hard drive or other storage device.
  - Loading the operating system
    - The BIOS loads the operating system into memory so that it can start running.

- It is critical that your BIOS knows where your OS is and boots into it for you.
- This is configured in the Boot Sequence or Boot Priority menu of BIOS.
  - There are two modes you'll see in bootup: UEFI (most modern) and Legacy.
  - Oftentimes compatibility issues during bootup can be resolved by toggling between UEFI and Legacy boot modes.

---

<!-- .element class="split-screen-with-title" -->
# CMOS

<div>

<div>

- Complementary metal-oxide-semiconductor (CMOS) holds BIOS configuration
  - Type of disk drives installed
  - System clock date & time
  - Boot sequence
- Reset CMOS memory by removing the CMOS battery to “clear” the CMOS, then reinserting it.

</div>

<div>

![Image](/ops-102-guide/curriculum/class-03/slides/assets/15_0.png)

</div>

</div>

NOTE:
SAY:
- CMOS stands for Complementary Metal-Oxide Semiconductor
- It is a small amount of memory on a computer motherboard that stores the Basic Input/Output System (BIOS) settings.
  - This includes the time, date, and hardware settings such as the boot order and the amount of memory installed.
- The CMOS battery is a small, coin-cell battery that provides power to the CMOS memory even when the computer is turned off.
  - This is necessary because the CMOS memory is volatile, which means that it loses its contents when the power is removed.
- Therefore by removing the CMOS battery you should be able to clear the BIOS time & date configuration because CMOS is volatile memory.
  - Motherboards vary between models, so there may be additional steps required to do so.
  - Another method is manipulating the CMOS jumper.
    - The CMOS jumper is typically located near the CMOS battery on the motherboard.
    - It is a small, three-pin jumper with a plastic cap.
    - The cap is usually labeled with the words "CLEAR" or "RESET."
    - To clear the CMOS memory, you will need to move the jumper from one set of pins to another.
      - The exact pins that you need to move the jumper to will be different depending on your motherboard.
      - You can usually find the instructions for clearing the CMOS memory in your motherboard manual.
- The CMOS battery typically lasts for several years, but it can eventually wear out.
  - If the CMOS battery dies, the BIOS settings will be lost and the computer will not be able to boot up properly.
- Some signs that your CMOS battery may be dying:
  - The time and date on your computer are incorrect.
  - The computer does not boot up properly.
  - The BIOS settings have been reset to their default values.
- You can buy a replacement CMOS battery at most electronics stores.

---

<!-- .element class="split-screen-with-title" -->
# Why Configure BIOS?

<div>

<div>

- Why might we alter BIOS settings?
  - Update firmware
  - Change boot order
  - Enable/disable a motherboard feature
  - Adjust a power, CPU, or RAM configuration setting
  - Clear the CMOS

</div>

<div>

![Image](/ops-102-guide/curriculum/class-03/slides/assets/16_0.png)

</div>

</div>

NOTE:
SAY:
- Why would you ever need to work on BIOS?
- Doesn't the computer boot into OS by itself?
- Here's a few reasons.
- Update firmware
  - The BIOS firmware is the software that controls the basic functions of your computer's motherboard. It is important to keep the BIOS firmware up to date to ensure that your computer is running with the latest security patches and bug fixes.
- Change boot order
  - The boot order is the order in which your computer searches for a bootable device when it starts up. You can change the boot order to boot from a specific device, such as a CD or DVD, or to boot from a network drive.
- Enable/disable a motherboard feature
  - The BIOS allows you to enable or disable certain motherboard features, such as virtualization support or overclocking.
- Adjust a power, CPU, or RAM configuration setting
  - The BIOS allows you to adjust the power settings for your CPU, the amount of RAM that is available to the operating system, and other settings.
- Clear the CMOS
  - The CMOS is a small amount of memory on your motherboard that stores the BIOS settings. If you need to reset the BIOS settings to their default values, you can clear the CMOS.

---

<!-- .element class="split-screen-with-title" -->
# Why Configure BIOS?

<div>

<div>

- What scenarios would prompt us to interact with BIOS?
  - Motherboard malfunction requiring firmware update
  - Booting into the wrong device
  - Feature not configured on motherboard
  - Overclocking
  - Resetting the CMOS to default settings

</div>

<div>

![Image](/ops-102-guide/curriculum/class-03/slides/assets/17_0.png)

</div>

</div>

NOTE:
SAY:
- Motherboard malfunction requiring firmware update
  - If your motherboard is malfunctioning, you might need to update the BIOS firmware.
  - The BIOS firmware is the software that controls the basic functions of your computer's motherboard.
  - Updating the BIOS firmware can fix bugs or add new features that can help to improve the stability of your computer.
- Booting into the wrong device
  - If your computer is booting into the wrong device, such as a CD or DVD drive, you can change the boot order in BIOS.
  - The boot order is the order in which your computer searches for a bootable device when it starts up.
  - You can change the boot order to boot from a specific device, such as a hard drive or a USB drive.
- Feature not configured on motherboard
  - If a feature is not configured on your motherboard, such as virtualization support, you can enable it in BIOS.
  - BIOS allows you to enable or disable certain motherboard features.
- Overclocking
  - If you want to overclock your CPU, you can do so in BIOS.
  - Overclocking is the process of increasing the clock speed of your CPU.
  - This can improve the performance of your computer, but it can also increase the heat output and instability of your system.
- Resetting the CMOS to default settings
  - If you make a change in BIOS that causes your computer to not boot up properly, you can reset the CMOS to restore the BIOS settings to their default values.

---
<!-- .element class="main-title" -->
# Demo and Lab Overview

NOTE:
DO:
- No need to go through ALL the steps.
- Review the lab tasks and submission instructions in Canvas
- Remind students to complete the reading assignment for next class before the upcoming lecture.

SAY:
- Next I'll prepare you for today's lab by showing you an example of BIOS and where all the important settings and information can be found.
- During the lab, you'll use your lab PC, so your BIOS menus will differ from what you see here.

- DO:
  - Navigate to a [Lenovo BIOS Simulator](https://support.lenovo.com/us/en/solutions/HT502745) (select IdeaCentre 310-15ASR (90G5)) and indicate where the below can be found. The simulator may not have all these.
    - Motherboard model
    - Processor specs
    - Total installed RAM
    - CPU Fan Speed
    - Processor Temperature
    - BIOS firmware version
    - Integrated Graphics Config
    - Menu to disable USB interfaces
    - Boot priority menu
    - Admin password menu
    - System Date & Time
    - Event Log
  - If time allows, also show students the [Phoenix BIOS Simulator](https://geekprank.com/bios/) for more exposure. Can't do much on this one though; pressing ENTER just reloads the whole emulator.
  - Demonstrate on your exposed lab PC (disconnect power, check static discharge, etc.)
    - Show students where the CMOS battery is
    - Remind them what the CMOS battery does (retain BIOS configuration memory such as time & date, etc.)
    - Carefully remove the CMOS battery. You may need to grab your precision screwdriver to wedge it off. There are two black plastic clamps holding it in place.
    - Return the CMOS battery.

---
