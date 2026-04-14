# Module 2, Lesson 05: Linux Administration & 15 Interview Scenarios

## 🎯 Objective
To master CLI administration, secure SSH workflows, and prepare for high-pressure technical interviews.

## 🧭 1. Core Navigation & Discovery
* `pwd`: Print Working Directory. Verifies your location before running destructive commands.
* `ls -la`: 
    * `-l`: Long listing (permissions, owner, group, size, date).
    * `-a`: Show hidden files (e.g., `.bashrc`, `.ssh`, `.git`).
* `cd -`: Toggles to the previous directory. Useful for jumping between `/etc` and `/var/log`.

## 🛠️ 2. File & Data Management
* `mkdir -p project/src/bin`: The `-p` flag creates parent directories if they don't exist.
* `mv`: Used for both moving and **renaming**.
* `rm -rf`: **Recursive** and **Force**. Standard for deleting directories, but use with extreme caution.

## 🔐 3. Security: The SSH Handshake (Automation Era)
I replaced HTTPS/PAT with **SSH** to secure my GitHub workflow. 
* **Mechanism**: Asymmetric Encryption (Ed25519).
* **Private Key**: Stored in `~/.ssh/id_ed25519`; it is never shared.
* **Public Key**: Uploaded to GitHub to verify identity.
* **DevOps Benefit**: Enables **Non-Interactive** authentication, which is mandatory for CI/CD pipelines.

---

## 🎙️ 15 Critical Interview Scenarios (Hands-on Prep)

**1. Q: The disk is 100% full. How do you find the largest files?**
**A:** `du -ah / | sort -rh | head -n 10`. This finds usage, sorts by size, and shows the top 10.

**2. Q: A developer says "The app is slow." Where do you start?**
**A:** I check system resources using `top` or `htop` for CPU/RAM spikes, then check `/var/log/syslog` for hardware/kernel errors.

**3. Q: How do you check if a specific port (like 80) is open?**
**A:** `netstat -tuln | grep :80` or `ss -tuln`.

**4. Q: You need to find all files modified in the last 24 hours. Command?**
**A:** `find /path/to/search -mtime -1`. Essential for identifying recent breaking changes.

**5. Q: How do you search for a specific error string across 50 different log files?**
**A:** `grep -r "ERROR_CODE_123" /var/log/app/`. The `-r` flag searches recursively.

**6. Q: What is the difference between `soft link` and `hard link`?**
**A:** Soft link (Symbolic) is a shortcut to a filename; if the file moves, the link breaks. Hard link points to the Inode (the data); the link remains valid even if the original name is deleted.

**7. Q: How do you run a command in the background so it survives a logout?**
**A:** Use `nohup command &` or run it inside a `tmux` or `screen` session.

**8. Q: A file has "Permission Denied" even for the owner. Why?**
**A:** The **Execute (x)** bit might be missing, or the file system is mounted as **Read-Only**.

**9. Q: How do you watch a log file update in real-time?**
**A:** `tail -f /var/log/syslog`.

**10. Q: How do you verify the Linux Kernel version?**
**A:** `uname -r`.

**11. Q: How do you find the process ID (PID) of a running application?**
**A:** `pgrep <app_name>` or `ps aux | grep <app_name>`. Essential for killing stuck processes.

**12. Q: What is a "Zombie Process" and how do you handle it?**
**A:** A process that has finished but still has an entry in the process table. You cannot "kill" a zombie; you must kill its **parent process** so the init system can clean it up.

**13. Q: How do you see the last 100 commands you typed?**
**A:** `history | tail -n 100`. Great for retracing your steps when you fix something but forget how.

**14. Q: A service won't start because the "Address is already in use." What do you do?**
**A:** Use `lsof -i :<port_number>` to find which PID is squatting on that port, then `kill -9 <PID>` to clear it.

**15. Q: How do you securely copy a file from one Linux server to another?**
**A:** I use `scp` or `rsync`. `rsync` is preferred because it is faster and supports resuming interrupted transfers.
