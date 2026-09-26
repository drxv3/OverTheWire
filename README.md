# 🛡️ OverTheWire: Bandit — Walkthroughs, Notes & Concepts

[![Platform](https://img.shields.io/badge/Platform-OverTheWire-blue.svg)](https://overthewire.org/wargames/bandit/)
[![Category](https://img.shields.io/badge/Category-Linux%20%2F%20CLI%20%2F%20Security-red.svg)]()
[![Progress](https://img.shields.io/badge/Levels%20Completed-0%2F34-success.svg)]()

This repository contains my writeups, technical notes, and conceptual breakdowns for the **OverTheWire Bandit** wargame. It is structured modularly with dedicated folders for each level, focusing on the core Linux concepts, tools, and security mechanisms behind each challenge.

---

## 🎯 About Bandit

OverTheWire Bandit is aimed at absolute beginners to intermediate users, teaching Linux fundamentals, command-line mechanics, and essential security concepts required for CTFs, penetration testing, and systems security.

### 🌐 Global Connection Parameters

* **Host:** `bandit.labs.overthewire.org`
* **Port:** `2220`
* **Default Protocol:** SSH

To log into any level, use:

```bash
ssh bandit<level>@bandit.labs.overthewire.org -p 2220
```

---

## 📁 Repository Architecture

The project is structured modularly. Every level has its own dedicated directory containing the writeup, relevant command syntax, and custom scripts:

```
overthewire-bandit/
├── README.md
├── scripts/
│   ├── brute_force_port.sh
│   └── helper_tools/
└── levels/
    ├── level00/
    │   └── README.md
    ├── level01/
    │   └── README.md
    ├── level02/
    │   └── README.md
    └── ... (through level33-34)
```

Each individual level writeup contains:

* **Objective:** Task description.
* **Core Concepts:** In-depth explanation of commands, kernel behavior, or protocols.
* **Command Breakdown:** Flags, piping, and syntax explanation.
* **Solution Steps:** Clean walkthrough of commands executed.

---

## 🗺️ Level Index & Core Concepts

| Level | Directory | Core Topic / Concepts | Status |
|---|---|---|---|
| 00 → 01 | `levels/level00/` | SSH Basics, Remote Access, Reading Standard Files (`cat`) | ⏳ In Progress |
| 01 → 02 | `levels/level01/` | Handling Dashes & Special Character Filenames (`./-`) | ⏳ In Progress |
| 02 → 03 | `levels/level02/` | Handling Whitespaces in Filenames (Escaping, Quotes) | ⏳ In Progress |
| 03 → 04 | `levels/level03/` | Hidden Files, Unix Dotfiles, `ls -la` | ⏳ In Progress |
| 04 → 05 | `levels/level04/` | Identifying File Types, MIME Types, `file` command | ⏳ In Progress |
| 05 → 06 | `levels/level05/` | Advanced File Discovery (find by size, permissions, properties) | ⏳ In Progress |
| 06 → 07 | `levels/level06/` | System-Wide Search (find by user, group, size, stdout/stderr redirection) | ⏳ In Progress |
| 07 → 08 | `levels/level07/` | Text Pattern Matching, Stream Processing (`grep`) | ⏳ In Progress |
| 08 → 09 | `levels/level08/` | Data Sorting, Finding Unique Lines (`sort`, `uniq -u`) | ⏳ In Progress |
| 09 → 10 | `levels/level09/` | Extracting Human-Readable Text from Binaries (`strings`) | ⏳ In Progress |
| 10 → 11 | `levels/level10/` | Base64 Encoding and Decoding (`base64 -d`) | ⏳ In Progress |
| 11 → 12 | `levels/level11/` | Caesar / ROT13 Substitution Ciphers (`tr`) | ⏳ In Progress |
| 12 → 13 | `levels/level12/` | Reversing Compression & Hex Dumps (`xxd`, `gzip`, `bzip2`, `tar`) | ⏳ In Progress |
| 13 → 14 | `levels/level13/` | Asymmetric SSH Keys, Key-Based Authentication (`ssh -i`) | ⏳ In Progress |
| 14 → 15 | `levels/level14/` | Network Sockets, Sending Data to Local Ports (`nc`, `telnet`) | ⏳ In Progress |
| 15 → 16 | `levels/level15/` | Encrypted Network Sockets, TLS/SSL Communication (`openssl s_client`) | ⏳ In Progress |
| 16 → 17 | `levels/level16/` | Port Scanning & TLS Handshakes (`nmap`, `openssl`) | ⏳ In Progress |
| 17 → 18 | `levels/level17/` | File Differencing, Analyzing Changes (`diff`) | ⏳ In Progress |
| 18 → 19 | `levels/level18/` | Bypassing `.bashrc` & SSH Forced Command Execution | ⏳ In Progress |
| 19 → 20 | `levels/level19/` | SUID (Set Owner User ID) Binaries & Privilege Execution | ⏳ In Progress |
| 20 → 21 | `levels/level20/` | Multi-Terminal Jobs, Local Netcat Listeners (`nc -lvnp`) | ⏳ In Progress |
| 21 → 22 | `levels/level21/` | Inspecting Scheduled Tasks & Crontab Entries (`/etc/cron.d/`) | ⏳ In Progress |
| 22 → 23 | `levels/level22/` | Shell Script Analysis, MD5 Hashing, Predictable Variables | ⏳ In Progress |
| 23 → 24 | `levels/level23/` | Cron Script Injection, Exploiting World-Writable Directories | ⏳ In Progress |
| 24 → 25 | `levels/level24/` | Network Port Brute-Forcing via Bash Loop Scripting | ⏳ In Progress |
| 25 → 26 | `levels/level25/` | Shell Escape via Pager (`more` / `vi` invocation in small terminal) | ⏳ In Progress |
| 26 → 27 | `levels/level26/` | Escaping Custom Shells & Privilege Escalation | ⏳ In Progress |
| 27 → 28 | `levels/level27/` | Version Control Inspection, Cloning Git Repositories via SSH | ⏳ In Progress |
| 28 → 29 | `levels/level28/` | Inspecting Git Commit Logs & Diff History (`git log`, `git show`) | ⏳ In Progress |
| 29 → 30 | `levels/level29/` | Inspecting Remote & Local Git Branches (`git branch -a`) | ⏳ In Progress |
| 30 → 31 | `levels/level30/` | Git Tags Analysis (`git tag`, `git show <tag>`) | ⏳ In Progress |
| 31 → 32 | `levels/level31/` | Pushing Code & Overriding `.gitignore` Constraints | ⏳ In Progress |
| 32 → 33 | `levels/level32/` | Escaping Uppercase Restricted Shells (`$0` variable exploit) | ⏳ In Progress |
| 33 → 34 | `levels/level33/` | Final Bandit Completion & Conclusion | ⏳ In Progress |

---

## 🛠️ Essential Linux Toolkit Used

* **Search & Filter:** `find`, `grep`, `sort`, `uniq`, `strings`, `cut`, `awk`, `sed`
* **Encoding & Compression:** `base64`, `xxd`, `tr`, `gzip`, `bzip2`, `tar`
* **Networking & Transport:** `ssh`, `scp`, `nc`, `nmap`, `openssl`, `curl`
* **System Administration & Permissions:** `cron`, `chmod`, `chown`, `id`, `file`
* **Version Control:** `git` (tags, logs, branches, push/pull)

---

## 🚀 Setup & Usage

To explore the writeups locally:

**Clone the repository:**

```bash
git clone https://github.com/<your-username>/overthewire-bandit.git
cd overthewire-bandit
```

**Navigate to the level of interest:**

```bash
cd levels/level00
cat README.md
```

---

## ⚖️ Ethics & Disclaimer

All writeups and materials in this repository are published strictly for educational and portfolio purposes. OverTheWire Bandit is designed to be solved through hands-on learning — if you are playing the game, use these writeups to understand the underlying theory rather than simply copy-pasting solutions.
