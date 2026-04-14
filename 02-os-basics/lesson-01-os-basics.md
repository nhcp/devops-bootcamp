# Module 2, Lesson 01: Operating System Fundamentals

## 🧠 Part 1: Comprehensive Theory
An Operating System (OS) is the primary software that manages computer hardware, software resources, and provides common services for computer programs.

### 1. The Kernel
The **Kernel** is the heart of the OS. It sits between the applications and the hardware. It handles:
* **Memory Management**: Allocating RAM to different processes.
* **Process Management**: Deciding which program gets the CPU's attention.
* **Device Drivers**: Communicating with hardware like disks and network cards.

### 2. User Space vs. Kernel Space
* **Kernel Space**: Reserved for the kernel, kernel extensions, and most device drivers. It is protected and has full hardware access.
* **User Space**: Where user applications (like your browser, Git, and Nginx) run. It must request permission from the kernel to access hardware via "System Calls."

### 3. Linux Distributions (Distros)
Since Linux is open-source, different organizations bundle the Kernel with different software. 
* **Ubuntu/Debian**: Uses `.deb` packages and `apt` manager.
* **RedHat/CentOS**: Uses `.rpm` packages and `yum/dnf` manager.

---

## 🎙️ Part 2: 15 Essential Interview Questions & Answers

| # | Question | Expert Answer |
| :--- | :--- | :--- |
| **1** | **What is the Linux Kernel?** | The core software that manages hardware-software communication. |
| **2** | **What is a System Call?** | The interface used by an app to request a service from the OS kernel. |
| **3** | **Difference between Shell and Kernel?** | The Shell is a user interface to the OS; the Kernel is the engine. |
| **4** | **What is an Absolute Path?** | A full path starting from root `/` (e.g., `/var/log/syslog`). |
| **5** | **What is a Relative Path?** | A path relative to your current folder (e.g., `./config.txt`). |
| **6** | **What is "Open Source"?** | Software where the code is public and can be modified by anyone. |
| **7** | **What is Multitasking?** | The OS's ability to switch between multiple tasks so fast they seem simultaneous. |
| **8** | **Who is the "Root" user?** | The administrative account with total control over the system. |
| **9** | **What is a Process?** | An instance of a program currently being executed. |
| **10** | **What is a Daemon?** | A background process that runs without user intervention (e.g., `sshd`). |
| **11** | **What is the Bootloader?** | Software that loads the OS into memory when you start the computer. |
| **12** | **What is Swap Space?** | Disk space used as "virtual memory" when physical RAM is full. |
| **13** | **What is a File System?** | A method of storing and organizing data on a disk (e.g., Ext4, XFS). |
| **14** | **GUI vs CLI for DevOps?** | CLI is preferred because it is faster, scriptable, and uses fewer resources. |
| **15** | **Why Linux for Servers?** | Because it is secure, stable, free, and designed for networking. |
