# Module 2, Lesson 03: Setup a Linux Virtual Machine

## 🎯 Objective
Learn the process of setting up a controlled, isolated Linux environment using virtualization technology.

## 🏗️ Traditional VM Setup (VirtualBox/VMware)
1. **Hypervisor Selection**: Using Type 2 Hypervisors like VirtualBox for local development.
2. **Resource Allocation**: Manually carving out CPU cores and RAM (e.g., 2GB or 4GB) from the host machine.
3. **ISO Installation**: Using a Linux image (Ubuntu) to boot and install the operating system.
4. **Virtual Disk**: Creating a dedicated storage space (VDI/VMDK) that lives as a file on the host computer.

## 💻 My Setup: WSL (Windows Subsystem for Linux)
While the bootcamp focuses on traditional VMs, I am using **WSL**, which provides a different approach:
* **Lightweight**: WSL shares the Windows kernel (WSL1) or runs a highly optimized utility VM (WSL2) that starts in seconds.
* **Resource Efficiency**: It dynamically uses RAM and CPU rather than "locking" it away like a traditional VM.
* **Integration**: It allows me to access Windows files directly from the Linux terminal and vice-versa.

## 🚀 Why this is important for DevOps
Whether using WSL or a traditional VM, a DevOps engineer must understand how to provision and manage a Linux environment. This knowledge is the foundation for managing Cloud instances (like AWS EC2) later in the course.
