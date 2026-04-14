# Module 2, Lesson 04: Linux File System Hierarchy

## 🧠 Part 1: Comprehensive Theory
In Linux, everything is a file. The system follows the **Filesystem Hierarchy Standard (FHS)** to organize data.

### 1. The Root ( / )
Unlike Windows, Linux has no drive letters (C:, D:). Everything is a branch of the root directory `/`.

### 2. Key Directories
* `/etc`: System configuration (DNS, Users, Network).
* `/var/log`: System and application logs (Troubleshooting ground).
* `/home`: User data.
* `/bin` & `/sbin`: System commands and binaries.

---

## 🎙️ Part 2: 15 Essential Interview Questions & Answers

| # | Question | Expert Answer |
| :--- | :--- | :--- |
| **1** | **What is /etc?** | The place for all system configuration files. |
| **2** | **Where are logs stored?** | In the `/var/log` directory. |
| **3** | **What is /root?** | The home directory for the root user only. |
| **4** | **What is /tmp?** | Temporary storage; usually cleared on reboot. |
| **5** | **What is /usr/bin?** | Most user-installed application commands live here. |
| **6** | **What is /dev?** | Contains files representing hardware devices (e.g., hard drives). |
| **7** | **What is /proc?** | A virtual filesystem with information about running processes. |
| **8** | **What is /mnt?** | Used for manually mounting external drives or filesystems. |
| **9** | **What is /boot?** | Contains the files needed to start the Linux system. |
| **10** | **What is a dot file?** | A hidden file (e.g., `.bashrc`) used for user settings. |
| **11** | **How to see hidden files?** | Use the `ls -a` command. |
| **12** | **What is a mount point?** | A directory where a separate filesystem is attached. |
| **13** | **What is /opt?** | Used for installing optional, third-party software. |
| **14** | **Difference between bin and sbin?** | `bin` is for everyone; `sbin` is for root system admin tools. |
| **15** | **"Everything is a file"?** | Yes, Linux treats hardware and even network sockets as files. |
