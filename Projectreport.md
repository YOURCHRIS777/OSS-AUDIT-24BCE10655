# Open Source Software Audit Report

## Course

Open Source Software Systems

## Student Name

CHRIS ARPAN DAVID 

## Selected Software

Python

## Environment

Linux (Ubuntu-based environment using GitHub Codespaces)

---

# 1. Introduction

Open Source Software (OSS) has transformed the way modern software is developed and distributed. Unlike proprietary software, open-source software allows users to freely access, study, modify, and distribute the source code. This openness encourages collaboration, innovation, and community-driven development.

Linux-based systems and open-source programming languages have become the backbone of modern computing infrastructure, powering servers, cybersecurity systems, artificial intelligence tools, and cloud platforms.

This project focuses on analyzing the open-source ecosystem of **Python**, a widely used programming language. The analysis includes studying its origin story, license model, ethical implications, Linux system footprint, and its role within the broader open-source ecosystem. In addition, several Linux shell scripts were developed to examine system properties and demonstrate practical scripting concepts.

---

# Part A – Open Source Background Study

## A1. Origin Story of Python

Python was created by **Guido van Rossum** in the late 1980s while he was working at the Centrum Wiskunde & Informatica (CWI) research institute in the Netherlands. The language was officially released in 1991.

At the time, many programming languages were complex and difficult for beginners to learn. Guido van Rossum wanted to design a language that prioritized **simplicity, readability, and productivity**. His goal was to create a language that allowed developers to write clear and understandable code with fewer lines.

Python was heavily influenced by earlier languages such as ABC, which emphasized simplicity and readability. However, Python improved upon these ideas by making the language more flexible and powerful.

One of the most important decisions made by Guido van Rossum was to release Python as **open-source software**. This allowed developers around the world to contribute to its development. Over time, a large global community formed around Python, continuously improving the language and expanding its ecosystem.

Today, Python is widely used in many fields including:

* Web development
* Artificial intelligence
* Data science
* Automation
* Cybersecurity
* Cloud computing

Its success demonstrates how open-source collaboration can lead to the development of powerful and widely adopted technologies.

---

## A2. License Analysis

Python is distributed under the **Python Software Foundation License**, which is a permissive open-source license.

This license allows users to:

* Use the software freely
* Modify the source code
* Redistribute modified versions
* Use the software for commercial purposes

The philosophy of open-source software is closely related to the **Four Freedoms of Free Software**, defined by the Free Software Foundation.

These freedoms include:

1. The freedom to run the program for any purpose.
2. The freedom to study how the program works and modify it.
3. The freedom to redistribute copies of the software.
4. The freedom to distribute modified versions of the software.

Python’s license supports these freedoms by allowing users to access and modify the source code.

### Comparison with Other Licenses

Open-source licenses can vary in their restrictions.

**GPL (General Public License)** requires that any modified versions of the software must also be released as open source.

**MIT License** is a permissive license that allows developers to modify and distribute software with minimal restrictions.

The Python Software Foundation License is similar to permissive licenses like MIT, allowing developers to use Python in both open-source and proprietary applications.

---

## A3. Ethical Reflection

Open-source software promotes values such as transparency, collaboration, and shared knowledge. When software is open-source, anyone can inspect the code, identify security vulnerabilities, and contribute improvements.

This transparency can improve software security because many developers can review the code and detect potential issues. In contrast, proprietary software hides its source code, making it difficult for users to verify how the software operates.

However, open-source software also raises ethical questions. For example, many companies build profitable products using open-source software created by volunteer developers. While this can lead to innovation, it may also raise concerns about whether contributors receive sufficient recognition or compensation.

Despite these challenges, open-source software remains one of the most powerful models for collaborative innovation. Communities around the world continue to contribute to open-source projects, improving technology for everyone.

---

# Part B – Linux Footprint of Python

The selected software was examined within a Linux environment to understand how it integrates into the system.

## Installation

Python is typically installed in Linux systems using a package manager.

Example installation command:

```
sudo apt install python3
```

The package manager automatically downloads and installs Python along with its dependencies.

---

## Binary Location

After installation, the Python executable is usually located at:

```
/usr/bin/python3
```

This location can be confirmed using the command:

```
which python3
```

---

## Configuration and Libraries

Python libraries and standard modules are stored in directories such as:

```
/usr/lib/python3
```

These directories contain the standard libraries used by Python programs.

---

## Log Files

System logs related to package installation and system events can be found in directories such as:

```
/var/log
```

These logs help administrators track software installations and system activity.

---

## Directory Permissions

Important system directories were analyzed to understand permissions, ownership, and disk usage. Examples include:

* /etc
* /var/log
* /home
* /usr/bin
* /tmp

These directories contain configuration files, system logs, user files, and executable programs.

Screenshots of these directory audits were captured using a shell script developed for this project.

---

# Part C – Open Source Ecosystem

Python is part of a large open-source ecosystem that includes many libraries, frameworks, and tools.

### Popular Python Libraries

Examples include:

* NumPy – numerical computing
* Pandas – data analysis
* TensorFlow – machine learning
* Flask – web development
* Django – web framework

These libraries expand Python’s capabilities and enable developers to build complex applications.

---

### Package Management

Python uses a package manager called **pip** to install external libraries.

Example command:

```
pip install numpy
```

Package managers allow developers to easily manage dependencies and update software.

---

### Community and Governance

The development of Python is managed by the **Python Software Foundation (PSF)**. The PSF coordinates development, organizes conferences such as **PyCon**, and supports the Python community.

Thousands of developers contribute to Python through bug reports, documentation improvements, and new features.

---

# Part D – Comparison with Proprietary Software

| Feature           | Python (Open Source) | MATLAB (Proprietary)  |
| ----------------- | -------------------- | --------------------- |
| Cost              | Free                 | Requires paid license |
| Source Code       | Available            | Not available         |
| Modification      | Allowed              | Restricted            |
| Community Support | Large open community | Vendor support only   |
| Transparency      | High                 | Limited               |

Python provides significant advantages due to its open-source nature. Developers can freely modify and distribute the software, which encourages innovation and experimentation.

Proprietary software such as MATLAB may provide professional vendor support, but it limits user freedom and access to source code.

Overall, open-source tools like Python provide greater flexibility and accessibility for developers and researchers.

---

# Part E – Shell Script Implementation

Five shell scripts were developed to analyze the Linux environment.

---

## Script 1 – System Identity Report

This script displays key information about the Linux system, including hostname, operating system details, kernel version, uptime, and the current user.

Commands used include:

* hostname
* uname
* uptime
* date
* whoami

<img width="1051" height="459" alt="Screenshot 2026-03-31 at 6 23 59 PM" src="https://github.com/user-attachments/assets/23524179-fa2a-4fff-a4e4-794a510faf13" />

---

## Script 2 – FOSS Package Inspector

This script checks whether Python is installed on the system and retrieves package information using the Linux package manager.

It uses conditional statements and command-line utilities such as `dpkg` and `grep`.

<img width="1070" height="766" alt="Screenshot 2026-03-31 at 6 25 03 PM" src="https://github.com/user-attachments/assets/9cf108b3-c7b8-4fed-9948-407f2f93e859" />

---

## Script 3 – Disk and Permission Auditor

This script examines several important Linux directories and reports their permissions, ownership, and disk usage.

A `for` loop is used to iterate through directories and analyze each one.

<img width="534" height="480" alt="Screenshot 2026-03-31 at 6 25 32 PM" src="https://github.com/user-attachments/assets/44c4395e-8d14-4064-bebf-fae2fb715f01" />

---

## Script 4 – Log File Analyzer

This script analyzes a Linux log file and searches for occurrences of a keyword such as "error". It counts the number of matches and displays recent log entries.

The script demonstrates the use of a `while read` loop and conditional logic.

<img width="768" height="218" alt="Screenshot 2026-03-31 at 6 36 25 PM" src="https://github.com/user-attachments/assets/a20e4794-9960-41c5-9805-88a6093737c8" />

---

## Script 5 – Open Source Manifesto Generator

This interactive script asks the user several questions about open-source software and generates a personalized manifesto based on their responses.

The script demonstrates user input, string concatenation, and file output operations.

<img width="662" height="338" alt="Screenshot 2026-03-31 at 6 32 06 PM" src="https://github.com/user-attachments/assets/11d1dbc5-7056-47e2-b1e5-67fa23e6025d" />


---

# Conclusion

This project provided practical exposure to open-source software and Linux system analysis. By studying Python and its ecosystem, the project demonstrated how open-source communities collaborate to build powerful technologies.

The development of shell scripts helped reinforce key Linux concepts such as loops, conditional statements, and system commands.

Open-source software continues to shape modern computing by promoting transparency, collaboration, and innovation. Python is a clear example of how community-driven development can create widely adopted and impactful technologies.

---

# Author

CHRIS ARPAN DAVID
