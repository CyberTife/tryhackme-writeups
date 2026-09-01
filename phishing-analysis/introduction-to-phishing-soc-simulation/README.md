# 🔎 Introduction to Phishing – SOC Simulation

## 📌 Overview

As part of my **Cyber Skills Bridge Internship Program**, I completed the **Introduction to Phishing SOC Simulation** on TryHackMe.

This practical exercise simulated a Security Operations Center (SOC) environment where I investigated multiple security alerts and identified genuine threats hidden among false-positive alerts.

Using the **TryHackMe SOC Simulator and Splunk**, I practiced alert triage, phishing investigation, security event analysis, true-positive and false-positive classification, and incident reporting.

---

## 🎯 Goal of the Task

The goal of this task was to investigate a simulated security environment and correctly identify malicious activity while filtering out false-positive alerts.

The exercise was designed to develop practical SOC Analyst skills, including:

- Security alert triage
- Phishing investigation
- SIEM analysis
- True-positive identification
- False-positive identification
- Incident investigation
- Security event analysis
- Incident reporting

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **TryHackMe SOC Simulator** | Simulated a SOC environment containing security alerts that required investigation and classification |
| **Splunk** | Used to search and analyze security events during the investigation |
| **Incident Reporting** | Used to document investigation findings and communicate the outcome |

---

## 🔍 Investigation Process

### 1. Alert Triage

I began by reviewing the alerts presented in the SOC simulation.

The environment contained a mixture of **true-positive and false-positive alerts**, requiring me to investigate the alerts before making a classification.

The objective was to determine which alerts represented genuine security incidents and which were benign.

---

### 2. Phishing Alert Investigation

A major part of the investigation involved phishing-related alerts, including:

> **Inbound Email Containing Suspicious External Link**

I examined the available information associated with the alerts to determine whether the activity should be classified as malicious or benign.

This required analyzing the available phishing indicators and considering the context surrounding the suspicious activity.

---

### 3. Splunk Investigation

I used **Splunk** to investigate relevant security events and gather supporting information.

The investigation involved searching through available events, examining relevant activity, and using the available evidence to support my alert classifications.

This provided practical experience with using a SIEM to investigate security events and assist with alert triage.

---

### 4. Alert Classification

After investigating the alerts, I classified them as either:

- **True Positive** – an alert correctly identified as representing malicious or suspicious activity.
- **False Positive** – an alert correctly identified as benign activity.

The SOC Simulator provided feedback on my classifications and allowed me to evaluate the accuracy of my investigation.

---

## 🚨 True Positive Alerts

I correctly identified **three true-positive alerts**.

| ID | Alert Rule | Severity | Type | Classification |
|----|------------|----------|------|----------------|
| 8815 | Inbound Email Containing Suspicious External Link | Medium | Phishing | ✅ Correct |
| 8816 | Access to Blacklisted External URL Blocked by Firewall | High | Firewall | ✅ Correct |
| 8817 | Inbound Email Containing Suspicious External Link | Medium | Phishing | ✅ Correct |

### Key Observation

The investigation highlighted how suspicious external links in inbound emails can be an important indicator when investigating potential phishing activity.

It also reinforced the importance of examining the context and available evidence surrounding an alert rather than relying only on the alert title or severity.

---

## ⚠️ False Positive Alert

I correctly identified one false-positive alert.

| ID | Alert Rule | Severity | Type | Classification |
|----|------------|----------|------|----------------|
| 8818 | Inbound Email Containing Suspicious External Link | Medium | Phishing | ✅ Correct |

This demonstrated the importance of validating alerts before escalating them as confirmed security incidents.

Correctly identifying false positives is important in SOC operations because unnecessary escalation can contribute to alert fatigue and consume valuable investigation time.

---

## 📊 Results & Performance

The simulation was successfully completed with the following results:

| Metric | Result |
|--------|--------|
| True Positive Identification Rate | **100%** |
| False Positive Identification Rate | **100%** |
| Alerts Closed | **4 alerts** |
| Mean Time to Resolve | **24 minutes** |
| Mean Dwell Time | **98 minutes** |
| Scenario Result | **Security breach prevented** |

The simulation confirmed that I successfully identified all the true-positive alerts and correctly classified the false-positive alert.

---

## 📸 Evidence

### 1. Scenario Completion

![Scenario Completed](screenshots/scenario-completed.png)

The simulation confirmed that the scenario was successfully completed and the security breach was prevented.

---

### 2. True Positive Identification

![True Positives](screenshots/true-positives.png)

The simulation recorded a **100% true-positive identification rate**.

---

### 3. False Positive Identification

![False Positives](screenshots/false-positives.png)

The simulation recorded a **100% false-positive identification rate**.

---

### 4. Performance Metrics

![Performance Metrics](screenshots/performance-metrics.png)

The final performance metrics showed:

- **4 alerts closed**
- **24 minutes mean time to resolve**
- **98 minutes mean dwell time**

---

## 🧠 What I Learned

This exercise strengthened my understanding of how SOC Analysts investigate and triage security alerts.

I learned how to:

- Analyze and triage security alerts.
- Distinguish true positives from false positives.
- Investigate phishing-related activity.
- Use Splunk for security event analysis.
- Identify phishing-related indicators.
- Validate suspicious activity using available evidence.
- Prioritize alerts during an investigation.
- Document investigation findings professionally.

One of my biggest takeaways was that **SOC analysis is not simply about detecting suspicious activity**. A SOC Analyst must validate alerts, investigate available evidence, distinguish malicious activity from legitimate behavior, and document the investigation accurately.

---

## 👨‍💻 SOC Analyst Skills Practiced

This exercise provided hands-on practice in:

- 🔎 Alert Triage
- 🎣 Phishing Analysis
- 🛡️ Security Operations
- 📊 SIEM Analysis
- 🔍 Splunk Investigation
- 🚨 Incident Investigation
- ✅ True Positive Identification
- ⚠️ False Positive Identification
- 📝 Incident Reporting
- 🧠 Evidence-Based Analysis

---

## 🎯 Key Takeaway

The simulation gave me practical experience working through a SOC alert queue and making investigation decisions based on available evidence.

It reinforced the importance of **accurate alert classification, efficient investigation, SIEM analysis, and clear incident documentation** in Security Operations.

---

## 📌 Lab Information

| Information | Details |
|-------------|---------|
| **Platform** | TryHackMe |
| **Pathway** | SOC 1 |
| **Room** | Introduction to Phishing |
| **Environment** | SOC Simulator + Splunk |
| **Program** | Cyber Skills Bridge Internship Program |
| **Status** | ✅ Completed |
