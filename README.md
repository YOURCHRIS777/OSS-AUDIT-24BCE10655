# OSS Audit Project – Linux Shell Script Analysis

**Student Name:** CHRIS ARPAN DAVID
**Course:** Open Source Software Systems
**Project Type:** Linux Environment Audit using Shell Scripts

---

## Project Overview

This project demonstrates the use of **Bash shell scripting** to analyze and interact with a Linux system.
The goal is to explore how open-source operating systems provide transparency and control through command-line tools.

Five different scripts were developed to inspect various aspects of the system such as system identity, installed software, disk usage, log analysis, and open-source philosophy generation.

These scripts showcase fundamental Linux concepts including:

* command substitution
* loops
* conditional statements
* file handling
* user interaction

---

## Repository Contents

Scripts included in this repository:

| Script          | Purpose                                                                                    |
| --------------- | ------------------------------------------------------------------------------------------ |
| **Scripts1.sh** | Displays system identity including hostname, OS, kernel version, uptime, and current user. |
| **Scripts2.sh** | Checks if a specific package is installed and prints information about it.                 |
| **Scripts3.sh** | Audits important system directories to show their permissions, owner, and disk usage.      |
| **Scripts4.sh** | Analyzes a Linux log file to detect occurrences of a keyword such as "error".              |
| **Scripts5.sh** | Interactively generates a personalized open-source manifesto and saves it to a file.       |

---

## How to Run the Scripts

Make the scripts executable:

```
chmod +x Scripts1.sh Scripts2.sh Scripts3.sh Scripts4.sh Scripts5.sh
```

Run the scripts using:

```
./Scripts1.sh
./Scripts2.sh
./Scripts3.sh
./Scripts4.sh /var/log/dpkg.log
./Scripts5.sh
```

---

## Script Descriptions

### Script 1 – System Identity Report

This script introduces the Linux environment by displaying key system information such as hostname, operating system details, kernel version, uptime, and the current logged-in user. It acts like a welcome screen that summarizes the identity of the system.

### Script 2 – FOSS Package Inspector

This script checks whether a selected open-source software package is installed on the system. If found, it retrieves package details and prints a description explaining the software's purpose.

### Script 3 – Disk and Permission Auditor

This script audits several important Linux directories and reports their disk usage, owner, group, and permission settings. It uses a loop to analyze multiple directories automatically.

### Script 4 – Log File Analyzer

This script reads a system log file and searches for a specific keyword such as "error". It counts the occurrences of the keyword and displays the most recent matching log entries.

### Script 5 – Open Source Manifesto Generator

This script interacts with the user by asking questions about their views on open-source software. Based on the responses, it generates a personalized manifesto and saves it as a text file.

---

## Learning Outcomes

Through this project the following Linux concepts were explored:

* Bash scripting fundamentals
* Conditional statements and loops
* System monitoring commands
* File input and output
* Linux log analysis
* Interactive scripting

---

## Conclusion

This project demonstrates how shell scripting can be used to automate system inspection and analysis tasks in Linux. It also highlights the philosophy of open-source software, emphasizing transparency, collaboration, and innovation.

---

## Author

**CHRIS ARPAN DAVID**
