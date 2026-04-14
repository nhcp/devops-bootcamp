# Module 2, Lesson 05: Linux Administration & Interview Prep

## 🎯 Objective
Master CLI administration and prepare for technical interviews with structured scenarios.

## 🧭 1. Core Navigation
* `pwd`: Print Working Directory.
* `ls -la`: List all files with details.
* `cd -`: Toggle to previous directory.

## 🔐 2. Security: SSH Handshake
* **Private Key**: `~/.ssh/id_ed25519` (Stored locally, never shared).
* **Public Key**: Uploaded to GitHub for passwordless authentication.
* **Benefit**: Essential for secure, automated CI/CD pipelines.

---

## 🎙️ 15 Critical Interview Scenarios

| # | Scenario / Question | Technical Answer / Command |
| :--- | :--- | :--- |
| **1** | **Disk is 100% full.** How to find the largest files? | `du -ah / | sort -rh | head -n 10` |
| **2** | **App is slow.** Where do you start? | Check `top` or `htop` for resources; check `/var/log/syslog` for errors. |
| **3** | **Check if Port 80 is open?** | `netstat -tuln | grep :80` or `ss -tuln`. |
| **4** | **Find files modified in last 24h?** | `find /path -mtime -1` (Finds recent breaking changes). |
| **5** | **Search "ERROR" in 50+ files?** | `grep -r "ERROR" /var/log/app/` (Recursive search). |
| **6** | **Soft Link vs. Hard Link?** | **Soft:** A shortcut. **Hard:** Points to the actual data (Inode). |
| **7** | **Run command in background?** | Use `nohup command &` or a `tmux`/`screen` session. |
| **8** | **"Permission Denied" for owner?** | Missing **Execute (x)** bit or **Read-Only** filesystem. |
| **9** | **Watch logs in real-time?** | `tail -f /var/log/syslog`. |
| **10** | **Verify Kernel version?** | `uname -r`. |
| **11** | **Find Process ID (PID)?** | `pgrep <app>` or `ps aux | grep <app>`. |
| **12** | **What is a Zombie Process?** | A finished process still in the table. Must kill its **parent**. |
| **13** | **See last 100 commands?** | `history | tail -n 100`. |
| **14** | **"Address already in use"?** | Use `lsof -i :<port>` then `kill -9 <PID>`. |
| **15** | **Secure copy between servers?** | Use `rsync` (faster) or `scp`. |

---

### 🚀 Troubleshooting Workflow
> **Interview Tip:** When asked to fix a problem, always follow the **Observe → Locate → Analyze** flow. 
> 1. Use `top` to observe. 
> 2. Use `cd /var/log` to locate. 
> 3. Use `grep` to analyze.
