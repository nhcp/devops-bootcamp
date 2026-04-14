# Module 2, Lessons 09 & 10: Accounts & Permissions

## 🧠 Part 1: Important Basic Theories
DevOps engineers prepare the infrastructure and must control who has access to it[cite: 232, 244].

### 1. Users and Groups
* **Users**: Individual identities (e.g., your `nhcp` account).
* **Groups**: Collections of users sharing the same access levels[cite: 244].

### 2. Permissions (rwx)
* **Read (4)**: View the file.
* **Write (2)**: Change the file.
* **Execute (1)**: Run the file as a program[cite: 245].



---

## 🎙️ Part 2: 15 Essential Interview Questions & Answers

| # | Question | Basic Technical Answer |
| :--- | :--- | :--- |
| **1** | **How to see permissions?** | `ls -l`. |
| **2** | **How to change permissions?** | `chmod`. |
| **3** | **How to change owner?** | `chown`. |
| **4** | **What is sudo?** | "SuperUser Do" - running commands with root power. |
| **5** | **How to add a user?** | `sudo adduser <name>`. |
| **6** | **What is chmod 755?** | Owner can do everything; others can only read and execute. |
| **7** | **What is chmod 600?** | Only the owner can read/write (private file). |
| **8** | **How to change group?** | `chgrp` or `chown :groupname`. |
| **9** | **What is a recursive change?** | Using `-R` to apply changes to all subfolders. |
| **10** | **Where are users stored?** | `/etc/passwd`. |
| **11** | **Where are groups stored?** | `/etc/group`. |
| **12** | **Where are passwords?** | `/etc/shadow`. |
| **13** | **How to delete a user?** | `deluser`. |
| **14** | **What is umask?** | The default permission set for new files. |
| **15** | **Why not use Root?** | For security; it's better to use a regular user with `sudo`[cite: 323]. |
