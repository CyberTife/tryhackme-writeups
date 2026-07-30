# Search Skills

## Overview

The **Search Skills** room introduces several online resources and tools that cybersecurity professionals use to gather information about internet-connected devices, malware, vulnerabilities, and Linux commands. These tools support research, threat intelligence, and vulnerability analysis.

---

## Learning Objectives

After completing this room, I was able to:

- Understand the purpose of cybersecurity search tools.
- Learn how Shodan indexes internet-connected devices.
- Explore how VirusTotal analyzes files and URLs.
- Understand the role of the CVE and CVSS systems.
- Use Linux man pages to access command documentation.

---

# What I Learned

## Shodan

Shodan is a search engine designed to discover internet-connected devices rather than websites.

It continuously scans the internet and indexes devices such as:

- IoT devices
- Servers
- Routers
- Industrial Control Systems (ICS)
- Traffic cameras

Shodan helps security professionals identify exposed systems and understand what services are publicly accessible.

---

## VirusTotal

VirusTotal is an online malware analysis platform.

It scans files and URLs using multiple antivirus engines and security vendors to determine whether they are malicious.

Security analysts often use VirusTotal during malware investigations and phishing analysis.

---

## Common Vulnerabilities and Exposures (CVE)

The CVE system provides standardized identifiers for publicly disclosed software vulnerabilities.

Each vulnerability receives a unique identifier, for example:

```text
CVE-2025-55182
```

Examples of well-known vulnerabilities include:

- Heartbleed
- Log4Shell
- Shellshock

---

## Common Vulnerability Scoring System (CVSS)

CVSS is a scoring system used to measure the severity of security vulnerabilities.

It helps organizations prioritize which vulnerabilities should be addressed first based on their potential impact.

---

## Linux Man Pages

Linux manual pages (man pages) provide built-in documentation for Linux commands.

Example:

```bash
man nc
```

This command displays the documentation for the `nc` (Netcat) command, including its usage and available options.

---

# Reflection

This room introduced me to several essential resources used by cybersecurity professionals. I learned that tools such as Shodan and VirusTotal can help gather valuable intelligence during investigations, while CVE and CVSS provide standardized ways to identify and assess vulnerabilities. I also discovered that Linux man pages are an excellent built-in reference for learning command-line tools.

---

# Key Takeaways

- Shodan indexes internet-connected devices rather than websites.
- VirusTotal analyzes files and URLs using multiple antivirus engines.
- CVEs provide unique identifiers for known vulnerabilities.
- CVSS helps prioritize vulnerabilities based on severity.
- Linux man pages are an essential reference for command-line usage.

---

# Skills Developed

- Open Source Intelligence (OSINT)
- Vulnerability Research
- Threat Intelligence
- Linux Command-Line Fundamentals

---

> **Source:** TryHackMe – Search Skills (Documented in my own words for learning purposes.)
