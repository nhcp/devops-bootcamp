# Module 2, Lesson 07: Package Management

## 🧠 Part 1: Comprehensive Theory
As a DevOps engineer, you are responsible for preparing the infrastructure (servers) on which the application is deployed[cite: 232]. Learning how to manage software through the CLI is a crucial prerequisite[cite: 233, 234].

### 1. What is a Package Manager?
A package manager is a tool that automates the process of installing, upgrading, configuring, and removing software packages[cite: 828]. It ensures that all necessary software and its specific versions are handled correctly without manual downloads.

### 2. The APT Package Manager (Ubuntu/Debian)
In this program, we primarily use **APT** (Advanced Package Tool), which is the standard for Ubuntu[cite: 829]:
* **apt update**: Updates the local list of available packages from the repositories[cite: 829].
* **apt install [pkg]**: Downloads and installs a specific software package[cite: 829].
* **apt remove [pkg]**: Removes an installed package from the system[cite: 829].
* **apt upgrade**: Upgrades all currently installed packages to their newest available versions[cite: 829].

### 3. Key Concepts for Automation
* **Repositories**: Centralized servers where software packages are hosted and verified.
* **Dependencies**: Software often requires other libraries to function; package managers resolve and install these automatically.
* **Sudo**: Administrative tasks like installing software must be run with `sudo` to modify system-level directories[cite: 835].



---

## 🎙️ Part 2: Top 15 Priority Interview Questions & Answers

| # | Question | Answer |
| :--- | :--- | :--- |
| 1 | **What is a Package Manager?** | A tool to automate the lifecycle of software (install, update, remove)[cite: 828, 829]. |
| 2 | **`apt update` vs `apt upgrade`?** | `update` refreshes the package list; `upgrade` installs the new versions[cite: 829]. |
| 3 | **How to install a package?** | Use the command `sudo apt install <package_name>`[cite: 829]. |
| 4 | **How to remove a package?** | Use the command `sudo apt remove <package_name>`[cite: 829]. |
| 5 | **What is a dependency?** | Additional software required by a program to function correctly. |
| 6 | **What is a Repository?** | A remote server where verified software packages are stored for download. |
| 7 | **Why use `sudo` with `apt`?** | Installing software changes system files, which requires root privileges[cite: 835]. |
| 8 | **How to install with no prompts?** | Use the `-y` flag (e.g., `sudo apt install pkg -y`). |
| 9 | **What is `apt autoremove`?** | Removes packages that were automatically installed to satisfy dependencies but are no longer needed. |
| 10 | **Where is the repo config?** | Usually located in `/etc/apt/sources.list`. |
| 11 | **What is a `.deb` file?** | The standard package format for Debian-based systems like Ubuntu. |
| 12 | **What is `dpkg`?** | The low-level tool that `apt` uses to handle the actual installation of `.deb` files. |
| 13 | **How to search for a package?** | Use `apt search <keyword>`. |
| 14 | **How to see installed packages?** | Use `dpkg -l`. |
| 15 | **Why automate `apt` in CI/CD?** | To ensure every server or container is built with the exact same software versions. |

