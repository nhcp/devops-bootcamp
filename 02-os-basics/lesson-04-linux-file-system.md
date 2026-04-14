# Module 2, Lesson 04: Linux File System Hierarchy

## 🎯 Objective
Understand how Linux organizes files and directories, and where important system data is stored.

## 📂 The Root Directory ( / )
In Linux, everything starts at the root directory, denoted by a single forward slash `/`. Unlike Windows (C: drive), Linux has a single unified hierarchy.

## 🗝️ Key Directories to Know
| Directory | Purpose |
| :--- | :--- |
| `/bin` | Contains binary executable programs (like `ls`, `cp`). |
| `/etc` | Contains system-wide configuration files (DNS, Network, Users). |
| `/home` | Personal folders for users (e.g., `/home/nhcp`). |
| `/root` | The home directory for the root (admin) user. |
| `/var/log` | Where the system keeps logs for troubleshooting applications. |
| `/tmp` | Temporary files that are usually deleted on reboot. |

## 🚀 DevOps Connection
As a DevOps engineer, you will spend most of your time in `/etc` changing configurations or in `/var/log` troubleshooting why an application isn't starting.
