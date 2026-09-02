# ⛓️ Cyber Kill Chain

## 📌 Overview

The **Cyber Kill Chain** is a cybersecurity framework that describes the different stages an attacker typically goes through to successfully compromise a target and achieve their objective.

Understanding these stages helps SOC Analysts identify attacks early, understand attacker behaviour, and determine where to look for evidence during an investigation.

## 🖼️ Cyber Kill Chain Diagram

![Cyber Kill Chain](./cyber-kill-chain.png)

---

## 🎯 Objectives

The objectives of this room were to:

- Understand the different stages of the Cyber Kill Chain.
- Learn how attackers progress from reconnaissance to their final objective.
- Understand how malware, exploits, and payloads are used during attacks.
- Learn about persistence and Command and Control (C2).
- Understand how defenders can detect attacker activity at different stages.
- Apply the Cyber Kill Chain to a simulated attack scenario.

---

## 🧠 Key Concepts

### 1. Reconnaissance 🔎

Reconnaissance is the stage where an attacker gathers information about the target before launching an attack.

The attacker may research:

- Employees
- Email addresses
- Domains
- Network information
- Technologies used by the organization

The goal is to understand the target and identify possible ways to attack it.

---

### 2. Weaponization 🛠️

During weaponization, the attacker prepares the tools and malicious components needed for the attack.

This can involve combining an exploit with a malicious payload.

#### Malware

**Malware** is software designed to damage, disrupt, spy on, or gain unauthorized access to systems.

#### Exploit

An **exploit** is code or a technique that takes advantage of a vulnerability or weakness in a system.

#### Payload

A **payload** is the malicious code or action that is delivered and executed on the target system.

---

### 3. Delivery 📩

Delivery is the stage where the attacker transmits the weaponized content to the target.

Examples include:

- Phishing emails
- Malicious attachments
- Malicious links
- Compromised websites
- Other delivery mechanisms

For a SOC Analyst, monitoring email, web, and network activity can help identify suspicious delivery attempts.

---

### 4. Exploitation 💥

Exploitation occurs when the attacker takes advantage of a vulnerability or weakness to execute malicious code or gain access to the target.

For example, an attacker may exploit a vulnerable application or trick a user into executing malicious content.

---

### 5. Installation / Persistence 🏠

After gaining access, the attacker attempts to maintain access to the compromised system.

This is commonly referred to as **persistence**.

Persistence allows the attacker to regain access even if the original method of compromise is no longer available.

Examples may include:

- Creating persistence mechanisms
- Modifying system settings
- Installing malicious software
- Creating scheduled tasks

---

### 6. Command and Control (C2) 📡

**Command and Control (C2)** is the communication between a compromised system and infrastructure controlled by the attacker.

C2 communication allows attackers to:

- Send commands to compromised systems
- Control infected machines
- Download additional malware
- Send information back to the attacker

SOC Analysts can investigate unusual network connections and communication patterns to identify possible C2 activity.

---

### 7. Actions on Objectives 🎯

This is the final stage of the Cyber Kill Chain.

At this stage, the attacker performs actions that achieve their ultimate objective.

Examples include:

- Stealing information
- Exfiltrating data
- Disrupting services
- Destroying data
- Deploying ransomware

The attacker's objective depends on their motivation and the target.

---

## 🔄 Cyber Kill Chain Flow

The Cyber Kill Chain can be summarized as:

**Reconnaissance**  
↓  
**Weaponization**  
↓  
**Delivery**  
↓  
**Exploitation**  
↓  
**Installation**  
↓  
**Command & Control (C2)**  
↓  
**Actions on Objectives**
