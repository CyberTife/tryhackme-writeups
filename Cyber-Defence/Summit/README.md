# 🏔️ Summit — Threat Intelligence & Detection

## 📌 Overview

The **Summit** room focuses on applying cybersecurity frameworks and threat intelligence concepts to understand and investigate adversary activity.

The room demonstrates how defenders can use information about attacker behaviour to identify suspicious activity and improve their ability to detect and respond to threats.

As a SOC Analyst, understanding attacker behaviour and knowing how to translate threat intelligence into detection opportunities is important for effective security monitoring.

---

## 🖼️ Summit

![Summit](./summit.png)

---

## 🎯 Objectives

The objectives of this room were to:

- Understand how threat intelligence can support security investigations.
- Analyse attacker behaviour and techniques.
- Identify indicators and activities associated with malicious behaviour.
- Understand how security teams can use intelligence to improve detection.
- Apply cybersecurity frameworks to an investigation.
- Understand the importance of correlating different pieces of evidence.

---

## 🧠 Key Concepts

### 1. Threat Intelligence

**Threat intelligence** is information about threats, threat actors, their techniques, and the indicators associated with malicious activity.

Threat intelligence can help security teams understand:

- Who may be targeting an organization.
- What techniques attackers may use.
- What infrastructure they may use.
- What indicators defenders should look for.
- How an attack may progress.

---

### 2. Indicators of Compromise

An **Indicator of Compromise (IOC)** is information that can provide evidence of potentially malicious activity.

Examples include:

- File hashes
- IP addresses
- Domain names
- Malicious URLs
- Suspicious files
- Network artifacts

SOC Analysts can use these indicators during investigations to determine whether systems may have been compromised.

---

### 3. Tactics, Techniques and Procedures

I learned that attackers use different **Tactics, Techniques, and Procedures (TTPs)** throughout an attack.

- **Tactic** – the attacker's objective or reason for performing an activity.
- **Technique** – the method used to achieve the objective.
- **Procedure** – the specific implementation of the technique.

Understanding TTPs allows defenders to focus on attacker behaviour rather than relying only on individual indicators.

---

## 🔎 Detection and Investigation

A SOC Analyst can use threat intelligence to guide an investigation.

A simplified investigation process is:

**Threat Intelligence**

↓

**Identify Relevant Indicators**

↓

**Search Security Logs**

↓

**Identify Suspicious Behaviour**

↓

**Correlate Evidence**

↓

**Map Activity to Attacker Techniques**

↓

**Detect and Respond**

This approach helps analysts understand whether individual alerts are connected to a larger attack.

---

## 🛡️ SOC Analyst Perspective

The room helped demonstrate the importance of using multiple sources of information during a security investigation.

Instead of investigating one indicator in isolation, a SOC Analyst can correlate:

- Endpoint activity
- Network traffic
- Authentication events
- Process execution
- File activity
- IP addresses
- Domains
- Other security alerts

Correlating these events can provide stronger evidence and help analysts understand the attacker's behaviour.

---

## 🧪 Practical Investigation Approach

When investigating suspicious activity, I learned that an analyst should consider the wider context.

For example:

**Suspicious File**

↓

**File Hash**

↓

**Process Execution**

↓

**Network Connection**

↓

**Destination IP / Domain**

↓

**Related User Activity**

↓

**MITRE ATT&CK Technique**

This type of correlation can help determine whether an event is isolated or part of a larger attack.

---

## 📝 What I Learned

I learned that **threat intelligence can provide valuable information that helps SOC Analysts understand and investigate potential attacks**.

I learned that indicators such as hashes, IP addresses, domains, and network artifacts can provide useful evidence during an investigation, but they become more valuable when they are correlated with other security events.

I also learned the importance of understanding **Tactics, Techniques, and Procedures (TTPs)**. Focusing on attacker behaviour allows security analysts to detect activity even when attackers change individual indicators such as file hashes or IP addresses.

Another important lesson was that effective detection requires more than identifying a single suspicious event. A SOC Analyst should investigate the surrounding context, correlate related events, and determine whether the activity matches known attacker behaviour.

---

## 🎯 SOC Analyst Takeaway

The main lesson I took from this room is that **good threat detection combines threat intelligence, indicators, behavioural analysis, and log correlation**.

A SOC Analyst should not only ask:

> **"Is this indicator malicious?"**

but also:

> **"What is happening around this indicator, and does it form part of an attack?"**

This approach can help analysts identify threats more accurately and respond to incidents more effectively.

---

## 🔑 Key Takeaway

The **Summit** room helped reinforce the importance of connecting threat intelligence with practical security monitoring.

By understanding attacker behaviour, identifying relevant indicators, and correlating security events, SOC Analysts can improve their ability to detect and investigate malicious activity.

---

## 🛠️ Skills Demonstrated

- Threat Intelligence
- IOC Analysis
- TTP Analysis
- Security Monitoring
- Log Analysis
- Threat Detection
- Incident Investigation
- MITRE ATT&CK Concepts
- SOC Analyst Investigation

---

## ⚠️ Disclaimer

This write-up documents my personal learning experience from the TryHackMe Summit room. It is intended for educational and portfolio purposes and does not include protected challenge answers or flags.
