# 🎯 MITRE ATT&CK Framework

## 📌 Overview

MITRE ATT&CK is a globally accessible knowledge base that documents real-world adversary tactics and techniques.

It provides a common language for cybersecurity professionals to understand, investigate, detect, and respond to attacker behaviour.

As a SOC Analyst, understanding MITRE ATT&CK helps me identify what an attacker is trying to accomplish, how they are carrying it out, and where evidence of their activity may appear in an environment.

---

## 🎯 Objectives

The objectives of this room were to:

- Understand the MITRE ATT&CK Framework.
- Learn about Tactics, Techniques, and Procedures (TTPs).
- Understand how attackers use different techniques throughout an attack.
- Learn how the MITRE ATT&CK Matrix organizes adversary behaviour.
- Understand how the ATT&CK Navigator can be used to visualize techniques.
- Learn how MITRE ATT&CK can support SOC investigations and detection.
- Understand the role of the Cyber Analytics Repository (CAR).
- Practice identifying attacker techniques based on a simulated APT scenario.

---

## 🧠 Key Concepts

### 1. Tactics

A **tactic** represents the attacker's goal or objective.

It answers the question:

> **Why is the attacker performing this activity?**

Examples of MITRE ATT&CK tactics include:

- Reconnaissance
- Resource Development
- Initial Access
- Execution
- Persistence
- Privilege Escalation
- Defence Evasion
- Credential Access
- Discovery
- Lateral Movement
- Collection
- Command and Control
- Exfiltration
- Impact

---

### 2. Techniques

A **technique** describes how an attacker achieves a particular tactical objective.

For example, an attacker may use **Phishing** to gain initial access to an organization.

Techniques provide defenders with more detail about the behaviour associated with an attack.

---

### 3. Sub-Techniques

Some MITRE ATT&CK techniques are divided into more specific **sub-techniques**.

Sub-techniques provide additional detail about how a technique is performed.

For example:

**Command and Scripting Interpreter**

can include sub-techniques such as:

- PowerShell
- Windows Command Shell
- Python
- JavaScript/JScript

Understanding sub-techniques can help SOC Analysts create more specific detections.

---

### 4. Procedures

A **procedure** describes the specific way an attacker or threat group has used a technique.

This provides practical context about how a technique may appear during a real attack.

The relationship can be simplified as:

**Tactic → Technique → Sub-technique → Procedure**

- **Tactic:** Why is the attacker doing it?
- **Technique:** How are they doing it?
- **Sub-technique:** What specific variation are they using?
- **Procedure:** How specifically are they carrying it out?

---

## 🧭 ATT&CK Navigator

The **MITRE ATT&CK Navigator** is a visualization tool that allows security professionals to create and analyze ATT&CK technique layers.

It can be used to:

- Visualize techniques used by threat actors.
- Map observed attacker behaviour.
- Identify techniques that may require additional detection.
- Compare threat actor activity.
- Support threat intelligence and detection engineering.

### Navigator Screenshot

![MITRE ATT&CK Navigator](./mitre.png)

---

## 🛡️ MITRE ATT&CK in SOC Operations

As a SOC Analyst, MITRE ATT&CK can help me:

- Investigate security alerts.
- Identify attacker behaviour.
- Map observed activity to specific techniques.
- Understand the possible stage of an attack.
- Improve detection and response.
- Communicate attacker activity using a common framework.

A simple SOC investigation workflow can be represented as:

**Alert → Investigate → Identify Behaviour → Map to MITRE ATT&CK → Detect → Respond**

---

## 🧪 Practical Scenario: APT28

In this room, I worked through a simulated scenario involving **APT28**.

The objective was to use the MITRE ATT&CK Navigator to identify techniques associated with the threat actor and determine what evidence a SOC Analyst should look for within an environment.

The investigation covered areas including:

- Reconnaissance
- Initial Access
- Execution
- Persistence
- Defence Evasion
- Discovery
- Lateral Movement
- Collection
- Exfiltration

This exercise helped me understand how a threat actor's behaviour can be mapped to MITRE ATT&CK techniques and how those techniques can guide security investigations.

---

## 🧠 What I Learned

I learned that **MITRE ATT&CK provides a structured way to understand attacker behaviour**.

I learned the difference between:

- **Tactics** — the attacker's goal.
- **Techniques** — how the attacker achieves that goal.
- **Sub-techniques** — more specific variations of techniques.
- **Procedures** — how a specific threat actor carries out a technique.

I also learned how the **MITRE ATT&CK Navigator** can be used to visualize the techniques associated with a threat actor.

The APT28 scenario helped me understand how a SOC Analyst can start with threat intelligence and work backwards to identify what activity should be searched for within an environment.

I also learned that MITRE ATT&CK can be useful during:

- Alert investigation
- Threat hunting
- Detection engineering
- Incident response
- Threat intelligence
- Security monitoring

### Key Takeaway

**MITRE ATT&CK helps security professionals understand what attackers do, why they do it, and how they carry it out.**

For a SOC Analyst, it provides a structured way to investigate suspicious activity, identify attacker techniques, and improve detection and response.

---

## 🛠️ Tools & Concepts

**Frameworks:**
- MITRE ATT&CK
- MITRE ATT&CK Navigator

**Concepts:**
- Tactics
- Techniques
- Sub-techniques
- Procedures
- TTPs
- Threat Intelligence
- Threat Hunting
- Detection Engineering
- Incident Response

---

## ⚠️ Disclaimer

This write-up documents my personal learning experience from the TryHackMe room. It is intended for educational and portfolio purposes and does not include protected flags or prohibited challenge answers.
