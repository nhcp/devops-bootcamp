# Module 2, Lesson 07: Package Management

## 🧠 Part 1: Core Theory
Package managers automate the installation, updating, and removal of software on Linux[cite: 828, 829]. As a DevOps engineer, you use these to prepare the server infrastructure where applications are deployed[cite: 232].

### 🛠️ Essential Commands (APT)
* **`apt update`**: Refreshes the local list of available software from the repositories[cite: 829].
* **`apt upgrade`**: Installs the latest versions of all currently installed packages[cite: 829].
* **`apt install [pkg]`**: Downloads and installs a specific software package[cite: 829].
* **`apt remove [pkg]`**: Uninstalls a software package from the system[cite: 829].

### 📍 Key Concepts
* **Repositories**: Centralized servers where verified software is stored for download[cite: 331, 103].
* **Dependencies**: External libraries required by a program; package managers resolve these automatically[cite: 294, 102].
* **Sudo**: Required for package management because it modifies system-level directories[cite: 835].



---

## 🎙️ Part 2: Top 10 Priority Interview Q&A

| # | Question | Answer |
| :--- | :--- | :--- |
| 1 | **What is a Package Manager?** | A tool to automate the installation and management of software[cite: 828]. |
| 2 | **`update` vs `upgrade`?** | `update` refreshes the list; `upgrade` installs new versions[cite: 829]. |
| 3 | **What is a Repository?** | A remote server where verified software packages are hosted[cite: 331]. |
| 4 | **How to install without prompts?** | Use the `-y` flag (e.g., `sudo apt install pkg -y`)[cite: 841]. |
| 5 | **What is a Dependency?** | Additional software needed by a program to function correctly[cite: 294]. |
| 6 | **How to remove a package?** | Use `sudo apt remove <package_name>`[cite: 829]. |
| 7 | **Why use `sudo` with `apt`?** | Changing system-wide software requires root privileges[cite: 835]. |
| 8 | **What is a .deb file?** | The standard package format for Debian-based systems like Ubuntu. |
| 9 | **How to search for a package?** | Use `apt search <keyword>`[cite: 755]. |
| 10 | **Why automate `apt`?** | To ensure infrastructure is consistent and job-ready[cite: 213, 214]. |
