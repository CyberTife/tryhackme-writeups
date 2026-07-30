# Offensive Security Introduction

## Overview

This room introduces the fundamentals of offensive security and explains how ethical hackers identify vulnerabilities before malicious attackers can exploit them.

---

## Learning Objectives

- Understand the concept of offensive security
- Differentiate offensive security from defensive security
- Learn how hidden web pages are discovered
- Explore directory enumeration using common security tools

---

## Key Concepts

### What is Offensive Security?

Offensive security is the practice of thinking like an attacker to discover weaknesses in systems, networks, or applications before real attackers can exploit them.

The goal is to identify and fix vulnerabilities to improve an organization's overall security.

---

### Offensive Security vs Defensive Security

| Offensive Security | Defensive Security |
|--------------------|-------------------|
| Finds vulnerabilities | Protects systems |
| Simulates attacks | Detects and responds to attacks |
| Thinks like an attacker | Thinks like a defender |

---

### Finding Hidden Web Pages

Not every web page is linked from a website's homepage. Hidden directories such as `/admin`, `/login`, or `/backup` may still be accessible if they exist.

Security professionals use directory enumeration tools to discover these hidden resources during security assessments.

---

### Directory Enumeration with Dirb

**Dirb** is a directory brute-forcing tool that searches for hidden files and directories on web servers.

Example:

```bash
dirb http://example.com
```

Dirb works by testing common directory names against a target website.

---

## What I Learned

- Offensive security focuses on identifying vulnerabilities before attackers do.
- Ethical hackers use attacker techniques to strengthen security.
- Hidden web pages may expose sensitive resources if not properly secured.
- Directory enumeration is an important reconnaissance technique.
- Tools like Dirb help discover hidden web content.

---

## Skills Developed

- Offensive Security Fundamentals
- Web Reconnaissance
- Directory Enumeration
- Basic Web Security

---

## Notes

These notes reflect my understanding after completing the **Offensive Security Intro** room on TryHackMe.
