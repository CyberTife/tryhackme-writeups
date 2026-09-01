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

Examples of tactics include:

- Reconnaissance
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

For example, an attacker may use **Phishing** as a technique to gain initial access.

Techniques provide defenders with more detail about the behaviour associated with an attack.

---

### 3. Procedures

A **procedure** describes the specific way an attacker or threat group has used a technique.

This provides more practical context about how a technique may appear during a real attack.

---

## 🔗 Tactics, Techniques and Procedures

The relationship can be simplified as:

```text
TACTIC
  ↓
Why is the attacker doing it?

TECHNIQUE
  ↓
How are they doing it?

PROCEDURE
  ↓
How specifically are they carrying it out?
