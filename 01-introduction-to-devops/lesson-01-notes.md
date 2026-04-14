# Module 1, Lesson 01: DevOps Fundamentals & Theory

## 🧠 Part 1: Important Basic Theories

### 1. What is DevOps?
DevOps is a cultural and technical movement that bridges the gap between **Software Development (Dev)** and **IT Operations (Ops)**. The goal is to deliver high-quality software faster and more reliably through automation and collaboration.

### 2. The SDLC (Software Development Life Cycle)
DevOps optimizes the SDLC, which includes:
* **Planning**: Defining requirements.
* **Development**: Writing code and version control.
* **Integration**: Testing and merging code.
* **Deployment**: Moving code to servers.
* **Monitoring**: Checking system health and user experience.



[Image of the DevOps infinity loop lifecycle]


### 3. The "Wall of Confusion"
Historically, Devs wanted **change** (new features) and Ops wanted **stability** (no crashes). This led to a "wall" where teams blamed each other. DevOps removes this wall so everyone is responsible for both speed and stability.

### 4. CI/CD (The Engine of DevOps)
* **Continuous Integration (CI)**: Automatically testing and merging code many times a day.
* **Continuous Delivery/Deployment (CD)**: Automatically preparing or sending code to production.

---

## 🎙️ Part 2: 15 Essential Interview Questions & Answers

| # | Question | Basic Technical Answer |
| :--- | :--- | :--- |
| **1** | **What is DevOps?** | A combination of culture and tools to automate and speed up software delivery. |
| **2** | **What is CI/CD?** | Automation that tests (CI) and deploys (CD) code changes automatically. |
| **3** | **What is "Toil"?** | Repetitive manual work that should be automated to save time. |
| **4** | **What is "Shift Left"?** | Testing for bugs and security issues earlier in the development process. |
| **5** | **How to handle a failed deployment?** | Use a **Rollback** to return to the last working version immediately. |
| **6** | **What is Infrastructure as Code (IaC)?** | Managing servers using configuration files (like Terraform) instead of manual clicks. |
| **7** | **DevOps vs Agile?** | Agile is about how we build software; DevOps is about how we deliver it. |
| **8** | **What is a Monolith?** | A single, giant application where all parts are tightly connected. |
| **9** | **What are Microservices?** | Breaking an app into small, independent pieces that talk to each other. |
| **10** | **What is Blue-Green Deployment?** | Having two identical servers; one is live, one is idle for testing the new update. |
| **11** | **What is a Canary Release?** | Releasing an update to 5% of users first to check for errors before everyone gets it. |
| **12** | **What is Monitoring?** | Tracking server health (CPU/RAM) and application logs to find problems fast. |
| **13** | **What is a Post-Mortem?** | A meeting after a failure to discuss what happened and how to prevent it. |
| **14** | **What is Idempotency?** | A command that produces the same result no matter how many times it is run. |
| **15** | **What is an Inode?** | A data structure in Linux that stores info about a file (except the name and data). |
