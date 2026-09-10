# IDS Fundamentals

## Overview

This lab introduced Intrusion Detection Systems (IDS), their deployment and detection methods, and how they support network security monitoring.

## What I Learned

I learned that an **Intrusion Detection System (IDS)** monitors activity and generates alerts when it identifies suspicious or abnormal behavior.

A useful analogy is:

- **Firewall = gatekeeper**
- **IDS = security camera**

A firewall controls whether traffic is allowed or blocked, while an IDS can inspect activity that has passed through security controls and alert analysts when suspicious behavior is detected.

## Types of IDS

### Host-Based IDS (HIDS)

A HIDS is installed on individual hosts and provides detailed visibility into activity on that specific system.

### Network-Based IDS (NIDS)

A NIDS monitors network traffic and provides a broader view of activity across the network.

## Detection Methods

### Signature-Based Detection

Uses known attack patterns or signatures.

**Strength:** Fast and effective against known threats.

**Limitation:** It may not detect new or zero-day attacks for which no signature exists.

### Anomaly-Based Detection

Uses a baseline of normal behavior and alerts when activity deviates from that baseline.

**Strength:** Can identify previously unknown or unusual activity.

**Limitation:** Can generate false positives when legitimate activity looks abnormal.

### Hybrid Detection

Combines signature-based and anomaly-based approaches.

## SOC Relevance

IDS alerts are useful starting points for SOC investigations. An analyst should not automatically treat every alert as a confirmed incident. The alert should be investigated and correlated with other evidence such as endpoint logs, firewall logs, DNS activity, authentication events, and network traffic.

## Key Takeaways

- IDS detects and alerts; it does not normally block traffic.
- HIDS focuses on individual hosts.
- NIDS focuses on network traffic.
- Signature detection is strong for known threats.
- Anomaly detection can help identify unusual or unknown activity.
- Hybrid detection combines both approaches.
- SOC analysts must validate and investigate IDS alerts.

## Evidence

![IDS Fundamentals Completion](../../../images/ids-fundamentals.png)

## Status

**Completed — 100%**
