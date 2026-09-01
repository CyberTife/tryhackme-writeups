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
- Understand the importance of attacker tools and TTPs.
- Understand why higher-level indicators are more difficult for attackers to change.
- Learn how SOC Analysts can use different indicators during investigations.

---

## 🔺 The Pyramid of Pain

The Pyramid of Pain represents different types of indicators that defenders can use to detect malicious activity.

The higher an indicator is on the pyramid, the more difficult it generally is for an attacker to change without changing their behaviour or methods.

![Pyramid of Pain](./pyramid-of-pain.png)

The progression from lower to higher levels is:

**Hash Values → IP Addresses → Domain Names → Host Artifacts → Network Artifacts → Tools → TTPs**

The higher we move up the pyramid, the more difficult and costly it generally becomes for an attacker to change their behaviour or methods.

---

## 🛠️ Tools and Techniques

During this room, I learned about different indicators and techniques that can be used to detect and investigate attacker activity.

Some of the concepts covered include:

- Hash analysis
- IP address analysis
- Domain analysis
- Host artifacts
- Network artifacts
- Tools
- Tactics, Techniques and Procedures (TTPs)

---

## 🧠 What I Learned

I learned that the **Pyramid of Pain** helps defenders understand which indicators are easier or harder for attackers to change.

I learned that **hashes** are useful for identifying known malicious files, but attackers can modify a file and generate a different hash.

I learned that **IP addresses** can be used to identify malicious infrastructure, but attackers can change IP addresses or use techniques such as **Fast Flux**.

I learned that **domain names** can be used as indicators of malicious activity and that attackers may use techniques such as **Punycode** and URL shorteners to make malicious links harder to identify.

I learned that **host artifacts** provide evidence of activity on a compromised system, including suspicious processes, files, and registry changes.

I also learned about **network artifacts**, including unusual User-Agent strings, URI patterns, HTTP requests, and Command-and-Control (C2) information.

The room helped me understand that higher-level indicators such as **Tools and TTPs** can be more valuable for detection because they are generally more difficult for attackers to change.

---

## 🎯 SOC Analyst Takeaway

As a SOC Analyst, I should not rely on a single Indicator of Compromise.

Instead, I can correlate different indicators such as:

**Hash → IP → Domain → Host Artifact → Network Artifact → Tools → TTPs**

This provides more context during an investigation and can make it more difficult for attackers to evade detection.

---

## 📚 Key Takeaway

The main lesson I took from this room is that **effective detection goes beyond identifying individual malicious files or IP addresses.**

Understanding attacker behaviour, tools, and TTPs can provide stronger and more resilient detection capabilities.

---

## ⚠️ Disclaimer

This write-up documents my personal learning experience from the TryHackMe room. It is intended for educational and portfolio purposes and does not include protected challenge flags or prohibited challenge answers.
