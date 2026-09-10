# Network Security Essentials

## Overview

This lab focused on understanding the main components of an enterprise network and how security analysts monitor and protect them.

## What I Learned

I learned that a network is made up of different assets including endpoints, file and database servers, application servers, Active Directory, routers, switches, and firewalls. Each component has a different security importance and can provide useful evidence during an investigation.

I learned that endpoints can be an initial entry point for attackers, while file and database servers contain valuable business data. Application servers such as web, email, and VPN servers are high-value targets because they are often exposed to external traffic. Active Directory is especially important because it manages identities, users, groups, computers, and access rights.

I also learned the importance of **network visibility**. Host-centric logs show what is happening on an individual system, while network-centric logs show communication between systems. Correlating both types of logs helps an analyst build an accurate incident timeline.

## Network Perimeter

The network perimeter separates the trusted internal network from the untrusted Internet. Common perimeter components include:

- Firewalls
- Routers and gateways
- DMZ
- VPN gateways

As a SOC analyst, monitoring the perimeter helps identify:

- Port scanning
- Brute-force attempts
- Exploitation attempts
- Suspicious outbound traffic
- Malware beaconing
- Possible data exfiltration

## Practical Investigation

I worked with firewall, IDS/WAF, and VPN logs and learned how to identify suspicious patterns.

Examples included:

- Repeated connections from one source to multiple ports → possible scanning
- Large numbers of authentication failures → possible brute-force activity
- IDS alerts identifying web attacks → possible exploitation
- Regular outbound connections → possible command-and-control beaconing

## SOC Relevance

This lab improved my ability to look beyond individual alerts and understand the wider network context. A SOC analyst needs to determine what happened, which system was affected, whether access was successful, and what happened after the initial activity.

## Key Takeaways

- You cannot effectively defend what you cannot see.
- Host and network logs complement each other.
- Firewall logs can provide early indicators of attacks.
- Perimeter monitoring is important for detecting reconnaissance and initial access.
- Correlation is more useful than investigating isolated events.

## Evidence

![Network Security Essentials Completion](../../../images/network-security.png)

## Status

**Completed — 100%**
