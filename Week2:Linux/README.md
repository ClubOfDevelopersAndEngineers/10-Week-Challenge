# Week 2: Linux

## Goal, Introduction, Important information
This week, our goal is to get you comfortable running Linux in a virtual environment so you can explore and experiment without affecting your main system. We’ll use VMware Workstation or VMware Player—a Type‑2 hypervisor that lets you run one or more “guest” operating systems on top of your existing “host” OS. VMware Workstation provides sandboxed environments for testing, development, and learning, with features like snapshotting and easy networking configurations.

**Over the next five days, you will:**
* Learn what VMware is and how it’s used
* Pick one of two Linux distributions (Ubuntu or Fedora) to install in VMware
* Follow both a video walkthrough and a written guide for your chosen distro
* Optionally explore installing Linux as your main OS (dual‑boot or native)

## Important Commands
Here are a list of some of the most common, basic Linux commands you can learn to get started:

**🔍 System Navigation & File Management**

| Command                      | Description                          |
| ---------------------------- | ------------------------------------ |
| ls                           | List files and directories           |
| cd \[dir]                    | Change directory                     |
| pwd                          | Print working directory              |
| mkdir \[dir]                 | Create a new directory               |
| touch \[file]                | Create an empty file                 |
| cp \[src] \[dest]            | Copy files/directories               |
| mv \[src] \[dest]            | Move/rename files/directories        |
| rm \[file]                   | Remove files                         |
| rm -r \[dir]                 | Remove directories recursively       |
| find \[dir] -name \[pattern] | Find files by name                   |
| locate \[filename]           | Quickly find files (uses a database) |

**📄 File Viewing & Editing**

| Command                   | Description               |
| ------------------------- | ------------------------- |
| cat \[file]               | View file contents        |
| less \[file]              | View file with navigation |
| head \[file]              | Show first 10 lines       |
| tail \[file]              | Show last 10 lines        |
| nano \[file]              | Simple text editor        |
| vim \[file] or vi \[file] | Advanced text editor      |

**📦 Package Management (Debian/Ubuntu)**

| Command                 | Description                       |
| ----------------------- | --------------------------------- |
| sudo apt update         | Update package list               |
| sudo apt upgrade        | Upgrade installed packages        |
| sudo apt install \[pkg] | Install a package                 |
| sudo apt remove \[pkg]  | Uninstall a package               |
| dpkg -i \[file.deb]     | Install a `.deb` package manually |

**🧑‍💻 User & Permissions Management**

| Command                        | Description               |
| ------------------------------ | ------------------------- |
| whoami                         | Show current user         |
| id                             | Show user ID and group ID |
| adduser \[name]                | Add a new user            |
| passwd \[user]                 | Change user password      |
| su \[user]                     | Switch user               |
| chmod \[perm] \[file]          | Change file permissions   |
| chown \[user]:\[group] \[file] | Change file owner/group   |

**🔐 Permissions & Security**

| Command    | Description                  |
| ---------- | ---------------------------- |
| chmod      | Change file permissions      |
| chown      | Change file owner            |
| sudo       | Run a command as root        |
| ufw        | Firewall management (Ubuntu) |
| ssh-keygen | Generate SSH key pair        |

**📆 System Information**

| Command          | Description                             |
| ---------------- | --------------------------------------- |
| alias ll='ls -l' | Create a shortcut command               |
| crontab -e       | Edit user’s cron jobs (scheduled tasks) |
| man \[command]   | Show manual for a command               |
| echo             | Print text                              |
| date             | Show current date and time              |
| env              | Show environment variables              |

## Setting up a Virtual Machine

### Introduction to VMware:

VMware Workstation (Windows/Linux) and VMware Player (free on Windows) are tools that let you create and manage virtual machines (VMs). You can allocate CPU, memory, storage, and networking to each VM independently, take snapshots to freeze and restore states, and share folders between host and guest machines.

---
**Option 1: Ubuntu in VMware**
* **YouTube Walkthrough:** “How to Install Ubuntu 24.04LTS on VMware Workstation Player on Windows 11” — a clear, step‑by‑step video showing how to download Ubuntu ISO, create a new VM, configure hardware settings, and complete the desktop install. ▶️ [https://youtu.be/SgfrHKg81Qc](https://youtu.be/SgfrHKg81Qc)

* **Written Guide:** Official Ubuntu Desktop install tutorial: detailed screenshots and instructions covering download, VM creation, and post‑install tips (VM Tools setup, shared folders). 🌐 [https://ubuntu.com/tutorials/install-ubuntu-desktop](https://ubuntu.com/tutorials/install-ubuntu-desktop)
---
**Option 2: Fedora in VMware**

* **YouTube Walkthrough:** “HOW TO: Install Linux Fedora 41 desktop on VMware” — up‑to‑date video (April 2025) that shows ISO download, VM setup, disk partition selection, and first‑boot configuration. ▶️ [https://youtu.be/7xVm3BhvBFw](https://youtu.be/7xVm3BhvBFw)

* **Written Guide:** LinuxFellas’ step‑by‑step Fedora install on VMware Workstation; Covers host prerequisites, VMware download/configuration, ISO installation, and VMware Tools integration. 🌐 [https://linuxfellas.com/install-fedora/](https://linuxfellas.com/install-fedora/)

---

**_Optional:_ Native or Dual‑Boot Installation**

If you’d prefer to run Linux directly on your hardware—either as your main OS or alongside Windows—here are two approaches:

* **Full native install**: Replace or wipe your existing system and install Linux as your only OS.
* **Dual‑boot setup**: Keep Windows and add Linux so you choose at startup.

  - Ubuntu Community Guide to Dual‑Boot Windows & Ubuntu → 🌐 [https://help.ubuntu.com/community/WindowsDualBoot](https://help.ubuntu.com/community/WindowsDualBoot)
  - Gcore’s concise dual‑boot walkthrough (partitioning, installer steps, GRUB) → 🌐 [https://gcore.com/learning/dual-boot-ubuntu-windows-setup](https://gcore.com/learning/dual-boot-ubuntu-windows-setup)

Choose the path that best fits your comfort level. If you’re new, the VMware approach is safest—your host remains untouched, and you can take snapshots before making any changes. Good luck, and happy scripting!

## Additional Resources
🧠 *Linux Essentials - Learning Resources:*

### Recommended by Tony Ziade:
* *ExplainShell (breaks down complex commands)*
  - 🔗 https://explainshell.com/
* *OverTheWire: Bandit (fun terminal challenges)*  
  - 🔗 https://overthewire.org/wargames/bandit/
* *Linux Journey (learn by levels)*
  - 🔗 https://linuxjourney.com/
* *Youtube Channels*
  - 🔗  https://www.youtube.com/@networkchuck
  - 🔗  https://www.youtube.com/@LinuxfoundationOrg
* *Test Linux in your browser:*
  - 🔗  https://bellard.org/jslinux/
* *Linux Visual Tree*
  - 🔗  https://rreinold.github.io/explore-linux/
  - 🔗  https://upload.wikimedia.org/wikipedia/commons/9/9a/Gldt1009.svg

---

### 📘 Beginner's Linux
* *Linux Survival* (interactive guide)  
  - 🔗 https://linuxsurvival.com/
* *Ubuntu Terminal Game* (official CLI tutorial)  
  - 🔗 https://ubuntu.com/tutorials/command-line-for-beginners
* *The Linux Command Line* (free book, PDF)  
  - 🔗 https://linuxcommand.org/tlcl.php

---

### 🎥 Video Courses
* *SSH for Beginners (freeCodeCamp)*  
  - 🔗 https://www.youtube.com/watch?v=hQWRp-FdTpc
* *SSH Crash Course (NetworkChuck)*  
  - 🔗 https://www.youtube.com/watch?v=ZtqBQ68cfJc

---

### 🧪 Distro Discovery
* *DistroSea* (compare and explore hundreds of Linux distros)  
  - 🔗  https://distrosea.com/
* *DistroWatch* (compare and explore hundreds of Linux distros)  
  - 🔗 https://distrowatch.com/
* *Linux Distro Chooser* (interactive quiz to find your distro)  
  - 🔗 https://distrochooser.de/
* *OSWatch* (modern distro browsing interface)  
  - 🔗 https://os.watch/

