# 🔺 Pyramid of Pain

## 📌 Overview

The **Pyramid of Pain** is a cybersecurity concept that illustrates how difficult it is for attackers to change the different indicators associated with their activities.

The higher an indicator is on the pyramid, the more difficult, time-consuming, and costly it becomes for an attacker to change or adapt it.

For defenders, this means that detection should not rely only on simple indicators that attackers can easily change. Combining multiple indicators and focusing on attacker behaviour can provide stronger and more resilient detection.

---

## 🎯 Objectives

The objectives of this room were to:

- Understand the Pyramid of Pain concept.
- Learn about different Indicators of Compromise (IOCs).
- Understand how hash values can be used during investigations.
- Learn how IP addresses can be used as indicators.
- Understand the role of malicious domain names.
- Learn about host artifacts and network artifacts.
- Understand how higher-level indicators increase the difficulty for attackers.
- Understand why combining multiple indicators can improve detection.

---

## 🧠 Key Concepts

### 1. Hash Values

Hash values are fixed-length values generated from data using a hashing algorithm.

Common hashing algorithms include:

- MD5
- SHA-1
- SHA-256

Hashes can be useful for identifying known malicious or suspicious files.

However, I learned that an attacker can modify a file, even slightly, and the resulting hash can become completely different.

Therefore, hash-based detection is useful for identifying known files, but hashes should not be relied upon as the only detection method.

---

### 2. IP Addresses

IP addresses can be used as indicators of malicious network activity.

Security teams can investigate or block known malicious IP addresses to help prevent communication with suspicious infrastructure.

However, attackers can change their infrastructure and use different IP addresses to evade detection.

I also learned about **Fast Flux**, where multiple IP addresses can be associated with a domain and changed frequently.

This can make simple IP-based blocking less effective.

---

### 3. Domain Names

Domain names can also be used as indicators of malicious activity.

Attackers may create domains that resemble legitimate websites or use techniques that make malicious domains more difficult to recognize.

I learned about:

- **Punycode**
- **URL shorteners**

These techniques can make malicious links appear more trustworthy or hide their actual destination.

---

### 4. Host Artifacts

Host artifacts are traces left on a system as a result of attacker activity.

Examples include:

- Suspicious processes
- Registry changes
- Malicious files
- Other system traces

Host artifacts can provide useful evidence during a security investigation because they provide more context about what happened on a compromised system.

---

### 5. Network Artifacts

Network artifacts are traces associated with network communication.

Examples include:

- Unusual User-Agent strings
- Command-and-Control (C2) information
- URI patterns
- HTTP requests

Network analysis tools such as **Wireshark, TShark, and Snort** can be used to investigate network artifacts.

---

## 📊 Indicators of Compromise

An **Indicator of Compromise (IOC)** is a piece of information that can provide evidence of potentially malicious activity.

Examples of IOCs include:

- File hashes
- IP addresses
- Domain names
- Host artifacts
- Network artifacts

SOC Analysts can correlate multiple indicators during an investigation instead of relying on a single IOC.

---

## 🔺 The Pyramid of Pain

The Pyramid of Pain demonstrates that different indicators create different levels of difficulty for attackers.

The general progression is:

```text
TTPs
  ↓
Tools
  ↓
Network Artifacts
  ↓
Host Artifacts
  ↓
Domain Names
  ↓
IP Addresses
  ↓
Hash Values

---

## 🛠️ Tools and Techniques

During this room, I learned how different indicators can be used to detect and investigate attacker activity.

Some of the concepts and techniques covered include:

- File hash analysis
- IP address investigation
- Malicious domain detection
- Punycode
- Fast Flux
- URL shorteners
- Host artifacts
- Network artifacts
- Command-and-Control (C2) activity
- Tactics, Techniques, and Procedures (TTPs)

Tools such as Wireshark, TShark, and Snort can help security analysts investigate network artifacts and identify suspicious communication.

---

## 🧠 What I Learned

This room helped me understand that not all Indicators of Compromise are equally valuable from a detection perspective.

I learned that **hashes are easy for attackers to change**, because modifying a file can result in a completely different hash. IP addresses and domains can also be changed or replaced when attackers modify their infrastructure.

As we move higher up the Pyramid of Pain, indicators become more difficult for attackers to change. **Host artifacts, network artifacts, tools, and TTPs provide more information about attacker behaviour and can therefore make detection more difficult for the attacker to evade.**

I also learned that SOC Analysts should avoid relying on a single IOC. Combining different indicators can provide stronger evidence during an investigation and help analysts understand what an attacker is doing rather than simply identifying one malicious file or connection.

The room also helped me understand why behavioural detection is important. Instead of only looking for known malicious hashes or IP addresses, defenders can look for patterns of behaviour associated with an attacker.

---

## 🔎 SOC Analyst Relevance

The Pyramid of Pain is useful to a SOC Analyst because it provides a way to think about the strength and usefulness of different indicators during detection and investigation.

For example:

- **Hash:** Can help identify a known malicious file.
- **IP Address:** Can help identify suspicious network communication.
- **Domain:** Can help identify malicious infrastructure.
- **Host Artifact:** Can reveal activity that occurred on a compromised system.
- **Network Artifact:** Can reveal suspicious communication patterns.
- **Tools:** Can help identify the software or utilities used by an attacker.
- **TTPs:** Can reveal the attacker's behaviour and methods.

Understanding these levels can help analysts move from simply identifying an IOC to understanding the broader behaviour of the attacker.

---

## 💡 Key Takeaway

The biggest lesson I took from this room is that **the higher we move up the Pyramid of Pain, the more difficult it becomes for an attacker to change the indicators associated with their activity.**

As a SOC Analyst, I should therefore look beyond simple indicators such as hashes and IP addresses and investigate **host artifacts, network artifacts, tools, and attacker TTPs** to build a stronger understanding of an incident.

---

## 📚 Room

**TryHackMe:** The Pyramid of Pain

**Module:** Cyber Defence Frameworks
