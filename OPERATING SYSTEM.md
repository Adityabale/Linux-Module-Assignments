# OPERATING SYSTEM



#### What is OS ?

An operating system (OS) is the software that manages all the hardware and software resources of a computer. Think of it as the brain of the computer, acting as a mediator between you (the user) and the computer's hardware. Without an OS, you wouldn't be able to run programs, save files, or even see anything on your screen.



#### What is Linux ?

Linux is a family of open-source, Unix-like operating systems. It's not a single product like Windows or macOS, but rather a core component—the Linux kernel—that is the foundation for a wide range of operating systems. These full operating systems, which bundle the Linux kernel with other software and utilities, are known as Linux distributions (or "distros").



The Linux kernel was created in 1991 by a Finnish student named Linus Torvalds. He wanted to create a free and open-source alternative to the Unix operating system



#### Key Features of Linux

Linux has become so popular and widely used because of its unique and powerful features:



1. Open Source: This is the most significant feature. The source code for Linux is freely available to everyone. Anyone can view, modify, and redistribute the code. This has led to a massive, worldwide community of developers who continuously work to improve and secure the OS.
2. Security: Because the code is open source, it's constantly being audited by thousands of developers. This collaborative approach means that security vulnerabilities are often discovered and patched much faster than in a closed, proprietary system. Linux is known for its robust security and is the platform of choice for many servers and mission-critical systems.
3. Stability and Reliability: Linux systems are incredibly stable and can run for years without needing a reboot. This is why it's the preferred operating system for servers, supercomputers, and other systems where uptime is essential.
4. Flexibility and Customization: This is where Linux truly shines. A single Linux kernel can be used to build a wide variety of operating systems, each tailored for a specific purpose. This has given rise to the concept of Linux distributions, which are essentially different versions of Linux.
5. Multi-User and Multi-Tasking: Like other modern operating systems, Linux is designed to handle multiple users and multiple programs running simultaneously without any conflict.
6. Portability: Linux can run on a vast range of hardware, from tiny embedded systems (like in your TV or car) to mobile phones (Android is built on the Linux kernel), to personal computers, and even the world's most powerful supercomputers.



The licensing under Linux runs under open source licenses such as

⦁	GNU-General Public License(GPL)

⦁	License Approved by Open Source Initiative (OSI).



Licensing and Distribution Model in Linux:

⦁	Licensing: Most Linux distributions are released under the GPL or other OSI-approved licenses, ensuring that users have access to the source code and the ability to modify and redistribute it.

⦁	Distribution: Linux distributions (distros) can be freely distributed, and users can create and share their own versions of Linux, contributing to the rich diversity of the Linux ecosystem.



#### Popular Distributions:



1. Ubuntu: One of the most popular and user-friendly distros, ideal for beginners. It's known for its ease of use and large community support.
2. Fedora: A community-driven distro that often introduces the latest technologies. It's a great choice for developers and those who want to use cutting-edge software.
3. Debian: The foundation for many other distros (including Ubuntu). It's known for its stability and is often used for servers.
4. Linux Mint: Another excellent choice for beginners, especially those transitioning from Windows, as its desktop environment is very familiar.
5. Red Hat Enterprise Linux (RHEL): A commercial, enterprise-focused distro known for its professional support and stability.



#### General Public License (GPL)

The GNU General Public License (GPL) is a widely used free software license that ensures end users have the freedom to run, study, share, and modify the software.

Key Features:

Copyleft: The GPL license is a "copyleft" license, meaning any derivative work based on GPL-licensed software must also be distributed under the same license. This ensures that the software remains free and open for all future users.

Freedom to Modify: Users can modify the source code and distribute their modifications, but they must also release the source code of their modified version.

No Proprietary Derivatives: GPL-licensed software cannot be integrated into proprietary (closed-source) software without violating the license.



#### The Open Source Initiative (OSI)

The Open Source Initiative (OSI) is a non-profit organization that promotes and protects open source software by reviewing and approving licenses that meet their definition of "open source."

Key Features:

Freedom to Use: OSI-approved licenses allow users to freely use the software for any purpose.

Freedom to Modify: Users can access the source code, make changes, and distribute those changes.

Freedom to Distribute: Users can distribute the software, whether it’s in its original form or with modifications, to anyone and for any purpose.

Variety of Licenses: OSI approves a variety of licenses, ranging from permissive ones like the MIT License, which allows proprietary use, to copyleft licenses like the GPL, which require derivative works to remain open source.



#### Types of Open Source licenses:



###### 1\. Copyleft Licenses (e.g., GNU GPL, LGPL)



* Core Philosophy: "Share-alike" or "reciprocal." The primary goal is to ensure that software, once released as open source, remains open source, even if it's modified and redistributed.



* Key Characteristic: If you distribute software that incorporates copyleft-licensed code, you must also make the source code of your modified or derivative work available under the same copyleft license.



* "Viral" Nature: This is often referred to as the "viral" nature of copyleft licenses. If you "infect" your project with GPL code, your entire project (or at least the parts linked to the GPL code) might need to be released under the GPL.



* Restrictions: While providing freedoms to users, they impose a "restriction" on developers who want to create proprietary (closed-source) derivatives. You cannot take GPL code, modify it, and then sell it as a proprietary product without releasing your modifications under the GPL.



* Purpose: To protect the "free" status of the software and prevent it from being absorbed into proprietary projects without contributing back to the open-source community.



###### 2\. Permissive Licenses (e.g., MIT, BSD, Apache)



* Core Philosophy: "Do whatever you want" (within reason). The primary goal is to maximize freedom for developers, allowing them to use the code in almost any way they choose, including in proprietary projects.



* Key Characteristic: They impose minimal restrictions on how the software can be used, modified, and redistributed. The main requirement is usually to include the original copyright and license notice.



* No "Viral" Nature: There is no requirement to release your modified or derivative work under the same open-source license. You can take permissive-licensed code, modify it, and then distribute your modified version as a proprietary, closed-source product.



* Restrictions: Very few, primarily just attribution.



* Purpose: To encourage widespread adoption and integration of the software, even by commercial entities that wish to keep their own modifications proprietary.



#### What is throughput ?

Throughput refers to the number of tasks, processes, or operations that a system can complete in a given unit of time.

In an OS, if a system can execute 50 user requests per second, its throughput is 50 requests/second.



###### Difference between latency and throughput

* Latency (or Response Time) is the time it takes for a single task to complete from start to finish.
* Throughput is about the quantity of tasks completed over time.





#### Here are the key functions of an operating system:



1. Resource Management: Hardware Resources: The OS manages and allocates CPU time, memory space, disk space, and I/O devices. It ensures that different programs and users running concurrently do not interfere with each other.
2. Software Resources: The OS handles the execution of programs, provides necessary services to applications, and efficiently manages system resources among all running applications.
3. Task Management: The OS is responsible for multitasking, which involves managing and scheduling the execution of multiple tasks. It keeps track of processor status, program status, and system functions.
4. Security: An operating system provides a secure environment within which system resources and user data are protected. This includes managing user access to programs and data, protecting against unauthorized access, and ensuring data integrity.
5. File Management: The OS manages files on various storage devices, organizes files in directories, and provides functions to create, move, delete, and access files. It also manages permissions and access rights for files and directories.
6. Device Control: The OS manages all device communication via respective drivers. It translates the user's read/write commands into device-specific calls, acting as a communicator between the hardware and the software.
7. User Interface: Operating systems provide interfaces through which users interact with computers. This can be a graphical user interface (GUI) like in Windows or macOS, a command-line interface (CLI) such as in Linux, or touch interfaces as seen in mobile operating systems like Android and iOS.
8. Networking: The OS handles networking capabilities, allowing different computing devices to communicate and share resources over a network. It manages the data exchange, network security, and connectivity protocols.
9. Program Execution: The OS loads programs into memory, sets up the execution stack, and handles the execution of applications. It provides mechanisms for process synchronization and inter-process communication.
10. Error Detection and Handling: The operating system continuously monitors the system for possible errors. It provides error-reporting methods to the users and takes appropriate actions to recover from system errors.



#### What is kernel ?

The kernel is the core component of an operating system (OS) that acts as the primary interface between the computer's software and its physical hardware. 💻 It is the first program loaded after the bootloader and remains in memory until the system is shut down. The kernel is like the central nervous system of a computer; it has complete control over everything and is responsible for managing all the essential operations



##### Key Functions of a Kernel



The kernel's main job is to manage the system's resources and facilitate communication between hardware and software. Its key functions include:



* Process Management: The kernel determines which processes get to use the central processing unit (CPU), for how long, and when. It ensures multiple programs can run at the same time, giving the illusion of simultaneous execution. This is a critical function for multitasking.



* Memory Management: The kernel allocates and manages the system's random access memory (RAM). It assigns specific memory spaces to each running process to prevent them from interfering with each other. The kernel also manages virtual memory, which allows the system to use more memory than is physically available by swapping data between RAM and the hard drive.



* Device Management: The kernel manages and controls all peripheral devices like keyboards, mice, monitors, and printers. It uses device drivers to communicate with these devices, abstracting the hardware's complexity so that applications don't need to know the specific details of how each device works.



* System Calls: The kernel provides a set of interfaces, known as system calls, that allow user applications to request services from the operating system, such as accessing files, reading from a disk, or using the network



###### Kernel Space

Definition: Kernel space (or kernel mode) is where the kernel (the core part of the operating system) operates. It has unrestricted access to the hardware and all system resources.



###### User Space

Definition: User space (or user mode) is the region of system memory where user applications and processes run. This space is protected and isolated from the kernel space, meaning that code running here cannot directly interact with the hardware or interfere with kernel operations.



Note: Kernel loads first into memory, when an OS is loaded and remains into memory until OS is shut down. The kernel has a process table that keeps track of all active processes.





##### Types of Kernels



Kernels are classified based on their architecture and how they manage system services.



* Monolithic Kernel: A single, large program where all OS services (file systems, device drivers, etc.) run in a single address space. This design is fast and efficient but can be unstable, as a single faulty driver can crash the entire system.



* Microkernel: A minimalist kernel that only includes the most essential services in the kernel space, such as inter-process communication and basic memory management. Other services run as separate processes in user space, making the system more modular, reliable, and secure. However, this design can be slower due to the overhead of message passing between services.



* Hybrid Kernel: This design combines elements of both monolithic and microkernels. It runs core services in the kernel space for speed, like a monolithic kernel, while keeping non-essential services in user space for better stability, like a microkernel. Most modern operating systems like Windows and macOS use this architecture



###### Users in Linux 

User is referred as individual who is interacting with the OS to perform various tasks, there are 3 types of users



1. Regular User: These are those users which are created during installation of Linux in this all the files and folders are stored in /home/ directory and they can not have access to directories of any other user. Their symbols is ‘$’ and can also be ‘%’
   
2. Root User: They are the super users that have all the admin privileges. Its symbol is ‘#’
   
3. Service User: This is widely used as server OS and services like e-mail and other applications have their own services account.



##### Directories in Linux



* /boot - This contains bootloader and kernel files, it also contains all the files that are needed during the boot of the system. 



* /home - This contains all the program files that are created by the user. It also contains user data, config files, user documents (all the personal files of a user).



* /bin(Binary Binaries) - This contains all the binary executable files, it also contains all the user commands in binary format like cd, pwd, mv, rm.



* /usr - It is also referred as Unix System Resources this contains all the user binaries, documentations, libraries, installed softwares and read only program data



* /etc - It is referred to as Editable Text Configuration that contains all the config files which are used by system services; it also contains system startup and system shutdown script that is used to start any program. 



* /var - It is referred to as Variables, contains all the variable data like log files generated by the system, cache files generated for applications.



* /tmp - It is referred to as temporary, contains temporary files created by various applications typically these are cleared when the system reboots.
