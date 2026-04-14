# Module 2, Lesson 07: Package Management

## 🧠 Part 1: Core Theory
Package managers are tools that automate installing, updating, and removing software on Linux. In DevOps, these are used to prepare the infrastructure where applications are deployed.

### 🛠️ Essential Commands (APT)
* **`apt update`**: Refreshes the local list of available software from the repositories.
* **`apt upgrade`**: Installs the latest versions of all currently installed packages.
* **`apt install [pkg]`**: Downloads and installs a specific software package.
* **`apt remove [pkg]`**: Uninstalls a software package from the system.



---

## 🎙️ Part 2: Top 10 Priority Interview Q&A

| # | Question | Answer |
| :--- | :--- | :--- |
| 1 | **What is a Package Manager?** | A tool to automate the installation and management of software. |
| 2 | **`update` vs `upgrade`?** | `update` refreshes the list; `upgrade` installs new versions. |
| 3 | **What is a Repository?** | A remote server where verified software packages are hosted. |
| 4 | **How to install without prompts?** | Use the `-y` flag (e.g., `sudo apt install pkg -y`). |
| 5 | **What is a Dependency?** | Additional software needed by a program to function correctly. |
| 6 | **How to remove a package?** | Use `sudo apt remove <package_name>`. |
| 7 | **Why use `sudo` with `apt`?** | Changing system-wide software requires root privileges. |
| 8 | **What is a .deb file?** | The standard package format for Debian-based systems like Ubuntu. |
| 9 | **How to search for a package?** | Use `apt search <keyword>`. |
| 10 | **Why automate `apt`?** | To ensure infrastructure is consistent and job-ready. |
