# Module 2, Lesson 11: Pipes and Redirects

## 🧠 Part 1: Important Basic Theories
These allow you to link small commands together to build powerful automation[cite: 246].

### 1. Redirects
* `>`: Overwrite a file with command output.
* `>>`: Add output to the end of a file (append).

### 2. Pipes ( | )
Takes the output of one command and gives it to another as input[cite: 246].

---

## 🎙️ Part 2: 15 Essential Interview Questions & Answers

| # | Question | Basic Technical Answer |
| :--- | :--- | :--- |
| **1** | **What does `|` do?** | Passes output from one command to another. |
| **2** | **What does `>` do?** | Saves output to a file (overwrites). |
| **3** | **What does `>>` do?** | Saves output to a file (adds to end). |
| **4** | **How to count lines?** | `cat file | wc -l`. |
| **5** | **How to find a word in a file?** | `grep "word" file`. |
| **6** | **What is stdout?** | Standard output (normal results). |
| **7** | **What is stderr?** | Standard error (error messages). |
| **8** | **What is stdin?** | Standard input. |
| **9** | **How to hide errors?** | `command 2> /dev/null`. |
| **10** | **What is /dev/null?** | The Linux "trash can" or black hole. |
| **11** | **How to sort a file?** | `cat file | sort`. |
| **12** | **How to see unique lines?** | `cat file | uniq`. |
| **13** | **How to see last 5 lines?** | `tail -n 5`. |
| **14** | **How to see first 5 lines?** | `head -n 5`. |
| **15** | **Why use pipes?** | To filter massive logs and find errors quickly. |
