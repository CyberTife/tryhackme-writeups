# 🕵️ Eviction — Threat Actor Analysis

## 📌 Overview

The **Eviction** room focuses on using the **MITRE ATT&CK Framework** and **ATT&CK Navigator** to understand the behaviour of a threat actor.

In this room, I worked through a simulated scenario involving **APT28**, where the objective was to identify the techniques the threat actor could use throughout an attack against an organization.

The exercise demonstrated how threat intelligence can be mapped to MITRE ATT&CK techniques and then used by a SOC Analyst to identify what activity to look for within an environment.

## 🖼️ ATT&CK Navigator

![Eviction - MITRE ATT&CK Navigator](./eviction.png)


---

## 🎯 Objectives

The objectives of this room were to:

- Understand how MITRE ATT&CK can be used to analyze a threat actor.
- Use the ATT&CK Navigator to visualize adversary techniques.
- Identify techniques associated with APT28.
- Understand how attacker techniques can appear during different stages of an attack.
- Determine what evidence a SOC Analyst should look for when investigating potential APT activity.
- Apply threat intelligence to security monitoring and investigation.

---

## 🧠 Threat Actor: APT28

The practical scenario focused on **APT28**, a threat actor whose activity was mapped using the MITRE ATT&CK Navigator.

The exercise required identifying different techniques that could be associated with the threat actor, including activities related to:

- Reconnaissance
- Initial Access
- Execution
- Persistence
- Defence Evasion
- Discovery
- Lateral Movement
- Collection
- Exfiltration

This demonstrated how a threat actor can use multiple techniques throughout an attack rather than relying on a single method.

---

## 🔎 Using MITRE ATT&CK Navigator

The **MITRE ATT&CK Navigator** provides a visual way to map and analyze techniques used by threat actors.

In this room, the Navigator layer helped identify techniques associated with APT28.

As a SOC Analyst, this type of information can be used to determine:

- What attacker behaviour to search for.
- Which logs and systems may contain evidence.
- Which techniques should have detection rules.
- What activity may indicate that an attacker has progressed further into the environment.

---

## 🔐 Initial Access and Social Engineering

The scenario demonstrated how attackers may use **social engineering** to gain initial access and convince users to execute malicious content.

User execution can become an important area for SOC Analysts to monitor because successful execution may lead to additional attacker activity.

Evidence that may be useful during an investigation includes:

- Suspicious email activity
- Malicious attachments
- Malicious links
- Unusual process execution
- Script execution
- Endpoint security alerts

---

## ⚙️ Execution and Scripting

The scenario also demonstrated the importance of monitoring **scripting interpreters**.

Attackers may use legitimate scripting functionality to execute commands or malicious scripts.

From a SOC perspective, suspicious scripting activity can be investigated by examining:

- Process creation events
- Command-line arguments
- Parent-child process relationships
- Script execution
- Endpoint telemetry

This highlights why monitoring behaviour can be more useful than relying only on file-based indicators.

---

## 🏠 Persistence and Registry Activity

Attackers may attempt to maintain access to a compromised system by modifying system configuration or registry locations.

Registry changes can therefore provide useful evidence during an investigation.

A SOC Analyst should investigate unusual registry modifications, especially when they are associated with suspicious processes or scripts.

---

## 🛡️ Defence Evasion

Attackers may use legitimate system binaries or other techniques to avoid security controls.

This means that simply detecting the execution of a legitimate system tool may not always be enough.

SOC Analysts should consider:

- Which process launched the binary.
- What command-line arguments were used.
- What the process attempted to access.
- Whether the activity is consistent with normal user behaviour.
- Whether the activity is connected to other suspicious events.

This demonstrates the importance of **contextual analysis** during alert investigation.

---

## 🔍 Discovery

Attackers commonly perform discovery after gaining access to learn more about the compromised environment.

The scenario demonstrated how tools and network activity can provide evidence of discovery activity.

Examples of information an attacker may attempt to discover include:

- Network configuration
- Hosts
- Users
- Systems
- Services
- Available resources

SOC Analysts can investigate unusual discovery commands, tools, and network traffic.

---

## 🔄 Lateral Movement

After compromising one system, an attacker may attempt to move to other systems within the environment.

This is known as **lateral movement**.

Remote services can provide attackers with methods for accessing additional systems.

From a SOC perspective, useful evidence may include:

- Unusual remote connections
- Authentication events
- New source and destination relationships
- Suspicious account usage
- Remote service activity

---

## 📂 Collection and Exfiltration

The scenario showed how an attacker may eventually target an organization's information repositories.

After locating valuable information, the attacker may collect it and attempt to move it outside the environment.

This can involve two important activities:

**Collection**

Gathering information that is valuable to the attacker.

**Exfiltration**

Transferring collected information out of the compromised environment.

SOC Analysts can investigate unusual data access, large data transfers, suspicious network connections, and communication with external infrastructure.

---

## 🧪 Investigation Approach

The room helped demonstrate a structured approach to investigating a potential threat actor.

A SOC Analyst can follow a process such as:

**Threat Intelligence**

↓

**Identify Threat Actor**

↓

**Map Techniques Using MITRE ATT&CK**

↓

**Identify Expected Attacker Behaviour**

↓

**Search Security Logs**

↓

**Correlate Evidence**

↓

**Detect and Respond**

This approach helps turn threat intelligence into practical security monitoring.

---

## 🧠 What I Learned

I learned how the **MITRE ATT&CK Framework and ATT&CK Navigator** can be used to analyze the behaviour of a specific threat actor.

I learned that an attacker can use multiple techniques throughout an attack, from gaining initial access to moving through a network and eventually achieving their objective.

The APT28 scenario helped me understand how threat intelligence can be converted into practical investigation questions. Instead of simply knowing that a threat actor exists, I can use MITRE ATT&CK to identify the techniques associated with that actor and determine what evidence I should search for.

I also learned the importance of monitoring activities such as **user execution, scripting, registry modifications, discovery, lateral movement, collection, and exfiltration**.

Another important lesson was that SOC Analysts should not investigate suspicious activity in isolation. Correlating multiple events can provide a clearer picture of the attacker's behaviour and help determine whether activity is part of a larger attack.

---

## 🎯 SOC Analyst Takeaway

The main lesson I took from this room is that **threat intelligence becomes more useful when it can be translated into observable attacker behaviour**.

MITRE ATT&CK provides the framework for describing that behaviour, while security monitoring and log analysis can help determine whether those techniques are actually occurring within an environment.

A SOC Analyst can therefore use:

**Threat Intelligence → MITRE ATT&CK → Detection → Investigation → Response**

to improve their ability to identify and respond to threats.

---

## 🔑 Key Takeaway

The **Eviction** room helped me understand how to use MITRE ATT&CK to move from knowledge about a threat actor to practical detection and investigation.

Understanding the techniques used by an attacker allows defenders to know **what to look for, where to look for it, and how different activities may be connected during an attack**.

---

## 🛠️ Skills Demonstrated

- MITRE ATT&CK
- ATT&CK Navigator
- Threat Actor Analysis
- Threat Intelligence
- TTP Analysis
- SOC Investigation
- Detection Concepts
- Adversary Behaviour Analysis
- Incident Investigation

---

## ⚠️ Disclaimer

This write-up documents my personal learning experience from the TryHackMe Eviction room. It is intended for educational and portfolio purposes and does not include protected challenge answers or flags.
