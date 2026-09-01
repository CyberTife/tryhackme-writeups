# ⛓️ Cyber Kill Chain

## 📌 Overview

The **Cyber Kill Chain** is a cybersecurity framework that describes the different stages an attacker typically goes through during an attack.

The framework helps security professionals understand an attacker's progression, identify where an attack may be detected, and determine where defensive controls can be applied.

As a SOC Analyst, understanding the Cyber Kill Chain can help me recognize suspicious activity earlier and know where to look for evidence during an investigation.

---

## 🎯 Objectives

The objectives of this room were to:

- Understand the Cyber Kill Chain framework.
- Learn the different stages of a cyber attack.
- Understand how attackers progress through an attack.
- Identify potential detection opportunities at different stages.
- Understand how the framework can support incident investigation.
- Learn how the Cyber Kill Chain can help SOC Analysts detect attacks earlier.

---

## 🧠 The Seven Stages of the Cyber Kill Chain

### 1. Reconnaissance

Reconnaissance is the stage where an attacker gathers information about a target before attempting to compromise it.

Information may include:

- Employees
- Email addresses
- Domains
- IP addresses
- Technologies in use
- Publicly available information

For a SOC Analyst, reconnaissance activity may provide early warning that an organization is being targeted.

---

### 2. Weaponization

During weaponization, the attacker prepares the tools, malware, exploit, or payload that will be used against the target.

Key concepts include:

- **Malware:** Malicious software designed to perform unauthorized or harmful actions.
- **Exploit:** Code or a technique used to take advantage of a vulnerability.
- **Payload:** The malicious action or code that executes after exploitation.

The attacker combines the necessary components to create a method of compromising the target.

---

### 3. Delivery

Delivery is the stage where the attacker transmits the malicious payload to the target.

Common delivery methods include:

- Phishing emails
- Malicious attachments
- Malicious links
- Compromised websites
- Removable media

SOC Analysts can monitor email security systems, web traffic, endpoint activity, and other security logs to identify suspicious delivery attempts.

---

### 4. Exploitation

Exploitation occurs when the attacker takes advantage of a vulnerability or weakness to execute malicious code or gain access to the target.

Examples may include:

- Exploiting vulnerable software
- Exploiting operating system vulnerabilities
- Exploiting applications
- Exploiting user interaction

Security teams can use vulnerability management, endpoint protection, and monitoring to reduce the likelihood of successful exploitation.

---

### 5. Installation

After successful exploitation, the attacker may install malware or establish a mechanism that allows them to maintain access to the compromised system.

This can include:

- Malware installation
- Backdoors
- Persistence mechanisms
- Malicious services
- Scheduled tasks

For a SOC Analyst, suspicious processes, files, services, registry modifications, and scheduled tasks can provide useful evidence during an investigation.

---

### 6. Command and Control (C2)

At this stage, the compromised system communicates with infrastructure controlled by the attacker.

Command and Control allows the attacker to:

- Send commands
- Control compromised systems
- Download additional tools or malware
- Receive information from the victim

SOC Analysts can investigate network traffic, DNS requests, IP addresses, domains, and unusual communication patterns to identify potential C2 activity.

---

### 7. Actions on Objectives

This is the final stage of the Cyber Kill Chain.

The attacker carries out their ultimate objective after gaining access and establishing control.

Possible objectives include:

- Data theft
- Data destruction
- Financial fraud
- Espionage
- Ransomware deployment
- Disruption of services

At this stage, security teams may observe data collection, exfiltration, system modification, or other signs of the attacker's final objective.

---

## 🔍 Detection Opportunities

The Cyber Kill Chain can help SOC Analysts identify opportunities to detect an attack at different stages.

Examples include:

| Kill Chain Stage | Possible Detection Area |
|---|---|
| Reconnaissance | Unusual scanning or information-gathering activity |
| Weaponization | Malware and threat intelligence analysis |
| Delivery | Email security and web filtering |
| Exploitation | Endpoint and vulnerability monitoring |
| Installation | Process, file, registry, and persistence monitoring |
| Command & Control | DNS and network traffic analysis |
| Actions on Objectives | Data access, collection, exfiltration, and impact |

The earlier an attack is detected, the greater the opportunity to prevent the attacker from reaching their final objective.

---

## 🧪 Example Attack Scenario

A simple example of the Cyber Kill Chain can be represented by a phishing attack:

**1. Reconnaissance**

The attacker identifies an employee and discovers their email address.

↓

**2. Weaponization**

The attacker prepares a malicious document or payload.

↓

**3. Delivery**

The attacker sends the malicious file through a phishing email.

↓

**4. Exploitation**

The victim opens the malicious attachment and the attacker exploits the target.

↓

**5. Installation**

Malware is installed on the victim's system to establish access.

↓

**6. Command & Control**

The compromised system communicates with attacker-controlled infrastructure.

↓

**7. Actions on Objectives**

The attacker attempts to steal sensitive information or disrupt the organization.

This example shows how the Cyber Kill Chain can be used to understand an attack from beginning to end.

---

## 🛠️ How the Cyber Kill Chain Helps a SOC Analyst

The framework provides a structured way to investigate suspicious activity.

A SOC Analyst can use it to:

- Understand the possible stage of an attack.
- Identify what evidence to search for.
- Correlate events from different security tools.
- Determine where defensive controls can be applied.
- Identify opportunities to stop an attack before it progresses.
- Communicate the progression of an incident clearly.

A simplified investigation process is:

**Alert → Investigate → Identify Attack Stage → Collect Evidence → Contain → Respond**

---

## 🧠 What I Learned

I learned about the different stages an attacker goes through to successfully compromise a target and achieve their objective.

I learned that the Cyber Kill Chain provides a structured way to understand an attack from the initial reconnaissance stage through to the attacker's final objective.

I also learned that each stage provides opportunities for defenders to detect and disrupt malicious activity.

The framework helped me understand why SOC Analysts need to look at more than one event or alert during an investigation. Different activities across multiple stages can be correlated to build a clearer picture of an ongoing attack.

I also learned the importance of identifying attacks as early as possible because stopping an attacker during an earlier stage can prevent them from progressing further into the environment.

---

## 🎯 SOC Analyst Takeaway

The main lesson I took from this room is that **understanding the attacker's journey helps defenders understand where and how to detect them.**

The Cyber Kill Chain can help me move from simply responding to individual alerts to understanding how multiple suspicious activities may be connected as part of a larger attack.

---

## 📚 Key Takeaway

The Cyber Kill Chain provides a structured model for understanding the progression of a cyber attack:

**Reconnaissance → Weaponization → Delivery → Exploitation → Installation → Command & Control → Actions on Objectives**

Understanding these stages can help security professionals identify attacks earlier, investigate incidents more effectively, and apply defensive controls at different points in the attack.

---

## ⚠️ Disclaimer

This write-up documents my personal learning experience from the TryHackMe room. It is intended for educational and portfolio purposes and does not include protected challenge flags or prohibited challenge answers.
