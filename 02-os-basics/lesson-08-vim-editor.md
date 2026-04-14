# Module 2, Lesson 08: Working with Vim Editor

## 🧠 Part 1: Important Basic Theories
Vim is the standard text editor for DevOps. Since most servers don't have a mouse (GUI), you must know how to edit files using only your keyboard[cite: 243].

### 1. The Two Main Modes
* **Command Mode**: For navigating and deleting.
* **Insert Mode**: For typing text (Press `i` to enter).

### 2. Why it matters
You will use Vim to edit Nginx configs, Dockerfiles, and automation scripts directly on remote servers[cite: 243, 251].

---

## 🎙️ Part 2: 15 Essential Interview Questions & Answers

| # | Question | Basic Technical Answer |
| :--- | :--- | :--- |
| **1** | **How to open a file?** | `vim filename`. |
| **2** | **How to start typing?** | Press `i`. |
| **3** | **How to exit Insert mode?** | Press `Esc`. |
| **4** | **How to save and quit?** | `:wq`. |
| **5** | **How to quit without saving?** | `:q!`. |
| **6** | **How to delete a line?** | `dd` in Command mode. |
| **7** | **How to undo?** | Press `u`. |
| **8** | **How to search for a word?** | `/word-to-find`. |
| **9** | **How to jump to bottom?** | `G`. |
| **10** | **How to jump to top?** | `gg`. |
| **11** | **How to copy a line?** | `yy`. |
| **12** | **How to paste a line?** | `p`. |
| **13** | **How to show line numbers?** | `:set number`. |
| **14** | **How to delete one character?** | `x`. |
| **15** | **Why Vim over Nano?** | It is faster for professional engineers once the shortcuts are memorized. |
