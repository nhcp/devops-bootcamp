# Module 2, Lesson 06: Essential Linux Commands - The Ultimate Reference

## 🧠 Part 1: Comprehensive Theory & Command Categories

Mastering the command line is an investment that pays off throughout your entire tech career. This resource provides the commands you need for everyday tasks and server administration.

### 🧭 1. Navigation & File Management
* `pwd`: **Print working directory** — shows your current path.
* `ls`: **List files and directories**.
    * `ls -l`: Long format (shows permissions, owner, size).
    * `ls -a`: Show hidden files (those starting with a dot).
    * `ls -h`: Human-readable sizes (KB, MB, GB).
* `cd [directory]`: **Change directory**.
    * `cd ..`: Go up one level.
    * `cd ~`: Go to home directory.
    * `cd -`: Go to previous directory.

### 📂 2. File Operations
* `cat [filename]`: Display entire file contents.
* `less [filename]`: View file with pagination (scrollable).
* `head [filename]`: Show first 10 lines.
* `tail [filename]`: Show last 10 lines.
* `tail -f`: **Follow file updates in real-time** (essential for troubleshooting logs).
* `mkdir [dirname]`: Create a new directory.
* `rm [filename]`: Remove/delete a file.
    * `rm -r`: Remove directory and its contents recursively.
    * `rm -f`: Force remove without confirmation.
* `cp [source] [dest]`: Copy files or directories.
* `mv [source] [dest]`: Move or **rename** files.
* `touch [filename]`: Create an empty file.
* `diff [file1] [file2]`: Compare two files and see differences.
* `wc [file]`: Count lines, words, and bytes.
    * `wc -l`: Prints the number of lines.
    * `wc -w`: Prints the number of words.
    * `wc -m`: Prints the character count.

### 🔍 3. Searching and Finding
* `grep [pattern] [file]`: Search for a specific pattern.
    * `grep -i`: Case insensitive search.
    * `grep -r`: Recursive search through folders.
* `find`: Search for files with various options (type, name, size).
    * Example: `find . -name "*.log"` searches current directory and subdirectories for any file ending in '.log'.

### ⚙️ 4. System & Process Management
* `ps`: Show current processes.
    * `ps -ef`: All processes in full format.
    * `ps aux`: Detailed process list (CPU/Memory/User).
* `top`: Real-time process monitor (dynamic dashboard).
* `kill [pid]`: Terminate a process using its Process ID.
* `df -h`: Show disk space usage in human-readable format.
* `free -h`: Show memory (RAM) usage.
* `uptime`: Show how long the system has been running.

### 🌐 5. Network Commands
* `ping [hostname]`: Test connectivity to a server.
    * Example: `ping -c 4 google.com` (limits test to 4 packets).
* `curl`: Transfer data from or to a server.
    * Example: `curl -I https://example.com` (checks if a site is up using a HEAD request).
* `netstat`: Displays network statistics.
    * `netstat -tuln`: `-t` (TCP), `-u` (UDP), `-l` (listening), `-n` (numerical addresses).
* `ip addr`: View IP addresses and network interfaces.

### 🖥️ 6. System Information & History
* `uname`: Show system information (e.g., `uname -a` for all).
* `who`: Show who is currently logged in.
* `hostname`: Show or set the system's host name.
* `history`: Show a list of previously executed commands.
    * `!!`: Execute the last command again.
    * `Ctrl + R`: Search through command history.

### 🔑 7. Root Access & Security
* `sudo [command]`: Run a command as the root user.
* `sudo su`: Become the root user (interactive session).
* `passwd`: Change the current user's password.
* `ssh user@hostname`: Connect to a remote server securely.
* `ssh-keygen`: Generate an SSH key pair for passwordless login.

### 📦 8. Package Management (APT)
* `apt update`: Update the local package list.
* `apt install [pkg]`: Install a new software package.
* `apt remove [pkg]`: Remove a software package.
* `apt upgrade`: Upgrade all installed packages to their latest versions.

### 🔗 9. Chaining Commands (The Real Power)
Linux commands become incredibly powerful when you chain them together using the **Pipe (`|`)** symbol.
* **Example 1: Find and Read All Text Files**
  `find -type f -name "*.txt" | xargs cat`
* **Example 2: Find, Filter, Sort, and Clean Errors**
  `find -type f -name "*.txt" | xargs cat | grep "ERROR" | sort -k4 | uniq -f3 > errors.log`
    * This finds all text files, reads them, searches for "ERROR", sorts them, removes duplicates, and saves the result to `errors.log`.

---

## 🎙️ Part 2: 50 Essential Interview Questions & Answers

| # | Question | Answer |
| :--- | :--- | :--- |
| 1 | How do you see hidden files? | `ls -a` |
| 2 | How do you watch a log file live? | `tail -f [filename]` |
| 3 | How to search text recursively? | `grep -r [pattern]` |
| 4 | Difference between `>` and `>>`? | `>` overwrites; `>>` appends to the end of the file. |
| 5 | How do you count lines in a file? | `wc -l [filename]` |
| 6 | How do you find files by name? | `find . -name "filename"` |
| 7 | How to return to the previous directory? | `cd -` |
| 8 | How to remove a non-empty directory? | `rm -r [dirname]` |
| 9 | How to check available disk space? | `df -h` |
| 10 | How to check RAM usage? | `free -h` |
| 11 | How to search command history? | `Ctrl + R` |
| 12 | How to execute the very last command? | `!!` |
| 13 | What does `top` do? | Real-time monitoring of processes, CPU, and RAM usage. |
| 14 | How to terminate a process by ID? | `kill [PID]` |
| 15 | How to see listening TCP/UDP ports? | `netstat -tuln` |
| 16 | How to test a URL without downloading? | `curl -I [URL]` |
| 17 | What is `sudo`? | "SuperUser Do" — runs a command with administrative privileges. |
| 18 | How to compare two files? | `diff [file1] [file2]` |
| 19 | How to see the first 10 lines of a file? | `head [filename]` |
| 20 | How to find the system hostname? | `hostname` |
| 21 | How to create a new folder? | `mkdir [name]` |
| 22 | What information does `uname -a` provide? | Kernel version, OS architecture, and system name. |
| 23 | How to rename a file? | `mv [old_name] [new_name]` |
| 24 | How to copy a directory? | `cp -r [source] [dest]` |
| 25 | How to count words in a file? | `wc -w` |
| 26 | What is `/dev/null`? | A special file that discards all data written to it (the black hole). |
| 27 | How to find files larger than 100MB? | `find . -size +100M` |
| 28 | How to see the last 50 lines of a log? | `tail -n 50 [file]` |
| 29 | How to run a command in the background? | Add an `&` at the end (e.g., `sleep 10 &`). |
| 30 | How to check CPU info? | `cat /proc/cpuinfo` or `lscpu`. |
| 31 | How to see who is logged in? | `who` |
| 32 | What is a "Pipe" (`|`)? | It sends the output of one command to the input of another. |
| 33 | How to search ignoring case sensitivity? | `grep -i [pattern]` |
| 34 | How to create an empty file? | `touch [name]` |
| 35 | How to view a file with pagination? | `less [file]` |
| 36 | How to clear the terminal screen? | `clear` or `Ctrl + L` |
| 37 | How to list all running processes? | `ps aux` or `ps -ef` |
| 38 | What is `chmod 755`? | Owner: rwx, Group: r-x, Others: r-x. |
| 39 | How to check your Linux Kernel version? | `uname -r` |
| 40 | How to view all network IP addresses? | `ip addr` |
| 41 | How to send exactly 4 ping packets? | `ping -c 4 [host]` |
| 42 | How to redirect only error messages? | `command 2> [file]` |
| 43 | What is a "Shebang"? | The `#!` at the top of a script to define the interpreter (e.g., `#!/bin/bash`). |
| 44 | How to see the path of a command? | `which [command]` |
| 45 | How to exit the current shell session? | `exit` or `Ctrl + D` |
| 46 | What is the IP for localhost? | `127.0.0.1` |
| 47 | How to list only directories? | `ls -d */` |
| 48 | How to find where a binary is located? | `whereis [name]` |
| 49 | How to create a symbolic (soft) link? | `ln -s [target] [link_name]` |
| 50 | How do you change your own password? | `passwd` |
