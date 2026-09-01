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

```text
TTPs
  ↑
Tools
  ↑
Network Artifacts
  ↑
Host Artifacts
  ↑
Domain Names
  ↑
IP Addresses
  ↑
Hash Values

---

## 🛠️ Tools and Techniques

During this room, I learned about different indicators and techniques that can be used to detect and investigate attacker activity.

Key concepts covered include:

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

I also learned that tools such as **Wireshark, TShark, and Snort** can be used to investigate network artifacts and suspicious network communication.

---

## 🧠 What I Learned

This room helped me understand that not all Indicators of Compromise are equally difficult for attackers to change.

I learned that **hashes are relatively easy for attackers to change** because modifying a file can result in a completely different hash. IP addresses and domain names can also be changed when attackers modify their infrastructure.

As we move higher up the Pyramid of Pain, the indicators become more difficult for attackers to change. **Host artifacts, network artifacts, tools, and TTPs provide more information about attacker behaviour and can make it more difficult for attackers to evade detection.**

I also learned that SOC Analysts should not depend on a single IOC. Combining different indicators can provide stronger evidence during an investigation and help analysts understand the broader activity taking place on a system or network.

Another important lesson was the value of **behaviour-based detection**. Instead of only looking for known malicious hashes, IP addresses, or domains, defenders can investigate patterns of behaviour associated with attackers.

---

## 🔎 SOC Analyst Relevance

The Pyramid of Pain is useful to SOC Analysts because it helps them understand the different types of indicators that can be used during detection and investigation.

For example:

- **Hash values** can help identify known malicious files.
- **IP addresses** can help identify suspicious network connections.
- **Domain names** can help identify malicious infrastructure.
- **Host artifacts** can reveal activity that occurred on a compromised system.
- **Network artifacts** can reveal suspicious communication patterns.
- **Tools** can help identify software used by an attacker.
- **TTPs** can reveal the attacker's behaviour and methods.

Understanding these indicators can help a SOC Analyst move beyond simply identifying an IOC and investigate the wider behaviour of an attacker.

---

## 💡 Key Takeaway

The main lesson I took from this room is that **the higher an indicator is on the Pyramid of Pain, the more difficult and costly it becomes for an attacker to change it.**

As a SOC Analyst, I should therefore look beyond simple indicators such as hashes and IP addresses and investigate **host artifacts, network artifacts, tools, and attacker TTPs** to build a stronger understanding of an incident.

---

## 📚 Room Information

**TryHackMe Room:** The Pyramid of Pain

**Module:** Cyber Defence Frameworks

**Focus:** Indicators of Compromise, Threat Detection, and Attacker Behaviour

---

## ⚠️ Disclaimer

This write-up documents my personal learning experience while completing the TryHackMe room.

It is intended for educational and portfolio purposes and does not include protected challenge flags or restricted walkthrough solutions.
