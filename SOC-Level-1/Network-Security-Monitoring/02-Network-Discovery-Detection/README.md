# Network Discovery Detection

## Overview

This lab focused on understanding how attackers discover systems, services, ports, and vulnerabilities and how a SOC analyst can detect that activity.

## What I Learned

I learned that attackers perform network discovery to identify accessible assets, IP addresses, open ports, operating systems, services, service versions, and potential vulnerabilities.

Defenders also perform discovery for legitimate reasons such as asset inventory, vulnerability management, attack-surface reduction, and identifying unnecessary exposed services. Because both attackers and defenders can generate scanning traffic, a SOC analyst must use context to distinguish malicious scanning from authorized activity.

## External vs Internal Scanning

### External Scanning

External scanning occurs when an external source scans an organization's public-facing assets. This normally represents reconnaissance before the attacker has gained a foothold.

### Internal Scanning

Internal scanning occurs when an internal/private source scans other internal systems. This can be more serious because it may indicate that an attacker has already gained access and is preparing for lateral movement.

## Horizontal vs Vertical Scanning

### Horizontal Scanning

The same source scans the **same destination port across multiple destination IP addresses**. This can be used to find systems exposing a specific service.

### Vertical Scanning

The same source scans **multiple ports on one destination IP**. This helps an attacker identify the services exposed by a specific host.

## Scanning Techniques

I learned how several common scans work:

- **Ping sweep:** Uses ICMP to identify live hosts.
- **TCP SYN scan:** Uses SYN packets to identify hosts and potentially open TCP ports.
- **UDP scan:** Uses UDP traffic to identify UDP services, although lack of response does not clearly prove that a port is open.

## Practical Analysis

I worked with exported firewall/SIEM logs and learned to examine source IP, source port, destination IP, destination port, protocol, and connection state.

I also learned that authorized vulnerability scanners should be known to the SOC and ideally excluded or tuned in detection rules to reduce false positives.

## SOC Relevance

Network discovery is important because it can be an early indicator of an attack. A SOC analyst should ask who is scanning, whether the source is external or internal, what systems and ports are being targeted, whether the activity is authorized, and whether there is evidence of follow-on activity.

## Key Takeaways

- Scanning is not automatically malicious; context matters.
- External scanning usually indicates reconnaissance.
- Internal scanning can indicate an attacker has already gained access.
- Horizontal scanning targets one port across many hosts.
- Vertical scanning targets many ports on one host.
- Detection should be tuned to reduce noise from authorized scanners.

## Evidence

![Network Discovery Detection Completion](../../../images/network-discovery.png)

## Status

**Completed — 100%**
