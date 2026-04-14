# Module 2, Lesson 02: Introduction to Virtualization

## 🧠 Part 1: Comprehensive Theory
Virtualization is the process of creating a software-based (virtual) version of something, like a server. It allows one physical machine to run multiple independent systems.

### 1. The Hypervisor
The Hypervisor is the software layer that manages VMs by distributing physical resources (CPU, RAM) from the **Host** machine to the **Guest** VMs.
* **Type 1 (Bare Metal)**: Runs directly on hardware (e.g., VMware ESXi). Best for production.
* **Type 2 (Hosted)**: Runs as an app on an OS (e.g., VirtualBox). Best for development.

### 2. Why DevOps uses Virtualization
* **Isolation**: Test code in safe, isolated environments without risking the host machine.
* **Efficiency**: Run many virtual servers on one physical machine to save money/space.
* **Snapshotting**: Capture the exact state of a machine before a risky change.

---

## 🎙️ Part 2: 15 Essential Interview Questions & Answers

| # | Question | Expert Answer |
| :--- | :--- | :--- |
| **1** | **What is a VM?** | A digital version of a physical computer running its own OS. |
| **2** | **What is a Hypervisor?** | Software that creates and runs virtual machines. |
| **3** | **Host vs Guest?** | Host is the physical hardware; Guest is the virtual OS. |
| **4** | **VM vs Container?** | VMs have their own OS; Containers share the host OS kernel. |
| **5** | **What is a VM Snapshot?** | A "save point" that allows you to revert the VM if things break. |
| **6** | **What is NAT Networking?** | Network Address Translation; VM uses host's IP for internet. |
| **7** | **What is Bridged Networking?** | VM gets its own IP on the physical network like a real computer. |
| **8** | **What is Provisioning?** | The act of allocating and setting up virtual resources. |
| **9** | **What is an ISO?** | A file containing the full image of an OS installation disk. |
| **10** | **VirtualBox vs Cloud?** | VirtualBox is local virtualization; Cloud is remote virtualization. |
| **11** | **What is Oversubscription?** | Assigning more virtual RAM than physical RAM to maximize usage. |
| **12** | **What is Headless Mode?** | Running a VM without a graphical window to save resources. |
| **13** | **What are Guest Additions?** | Driver packages that improve VM performance and resolution. |
| **14** | **What is Live Migration?** | Moving a running VM from one host to another with zero downtime. |
| **15** | **What is a Virtual Hard Disk?** | A file on the host (e.g., .vmdk) that acts as the VM's storage. |
