# Module 2, Lesson 03: Setup a Linux VM & WSL

## 🧠 Part 1: Comprehensive Theory
Setting up a controlled, isolated Linux environment is the first step in any DevOps workflow.

### 1. Resource Allocation
When setting up a VM, we must decide:
* **CPU**: How many cores to borrow from the host.
* **RAM**: 2GB is minimum for Linux CLI; 4GB+ for heavy tasks.
* **Storage**: Usually "Dynamically Allocated" (the file grows only as you add data).

### 2. WSL (Windows Subsystem for Linux)
Instead of a traditional Type 2 Hypervisor, many use WSL. 
* **WSL2** uses a real Linux kernel running inside a very lightweight utility VM managed by Windows.
* **Benefit**: Extreme speed and direct access to Windows files.

---

## 🎙️ Part 2: 15 Essential Interview Questions & Answers

| # | Question | Expert Answer |
| :--- | :--- | :--- |
| **1** | **Why use WSL over VirtualBox?** | It is much faster and uses significantly less RAM/CPU. |
| **2** | **How to update Linux?** | Using the package manager: `sudo apt update && sudo apt upgrade`. |
| **3** | **What is an SSH Key?** | A secure way to log in without a password using cryptography. |
| **4** | **Public vs Private Key?** | Public key goes on the server; Private key stays on your machine. |
| **5** | **What is a "Terminal"?** | The interface where you type commands to talk to the shell. |
| **6** | **How to find your IP?** | Run `ip addr` or `ifconfig`. |
| **7** | **What is a "Package"?** | A compressed file containing an app and its instructions. |
| **8** | **What is a Repo?** | A central server where Linux packages are stored for download. |
| **9** | **What is sudo?** | "SuperUser Do" – allows you to run commands as root. |
| **10** | **How to install Git?** | `sudo apt install git`. |
| **11** | **How to exit a terminal?** | Type `exit` or press `Ctrl+D`. |
| **12** | **What is an LTS release?** | Long-Term Support; versions stable for 5-10 years. |
| **13** | **How to shut down WSL?** | Run `wsl --shutdown` in Windows PowerShell. |
| **14** | **Where are Windows files?** | Located in `/mnt/c/` within the WSL environment. |
| **15** | **Why use a VM for DBs?** | To ensure the database has its own dedicated resources and security. |
