# Man-in-the-Middle Detection

## Overview

This lab focused on detecting Man-in-the-Middle (MITM) activity, particularly ARP spoofing and DNS spoofing, using network traffic analysis.

## What I Learned

A **Man-in-the-Middle (MITM)** attack occurs when an attacker secretly positions themselves between two communicating parties and intercepts or potentially modifies their communication.

Common MITM techniques covered included:

- Packet sniffing
- Session hijacking
- SSL stripping
- DNS spoofing
- IP spoofing
- Rogue Wi-Fi access points

## ARP and ARP Spoofing

I learned that ARP maps an IP address to a MAC address on a local network.

ARP spoofing abuses the lack of authentication in ARP. An attacker can send fake ARP replies and convince a victim that the attacker's MAC address belongs to the legitimate gateway.

```text
Victim → Attacker → Gateway
```

The attacker is then positioned in the communication path.

## ARP Spoofing Indicators

During investigation, useful indicators include:

- Duplicate IP-to-MAC mappings
- Unsolicited ARP replies
- Abnormally high ARP traffic
- Traffic being routed through a suspicious MAC address
- Multiple MAC addresses associated with the gateway IP

## DNS Spoofing

I also learned how DNS spoofing can redirect a victim to an attacker's system.

```text
Victim requests website
        ↓
Attacker sends fake DNS response
        ↓
Victim receives attacker-controlled IP
        ↓
Victim connects to attacker
```

Important indicators include multiple DNS responses for the same query, responses from an unexpected source, very short TTL values, and unsolicited DNS responses.

## Wireshark Investigation

I used Wireshark filters to narrow traffic during investigation, including:

```text
arp.opcode == 2
```

```text
dns
```

```text
dns.flags.response == 1
```

These filters helped isolate ARP and DNS traffic and identify abnormal responses.

## SOC Relevance

MITM detection is important because it can indicate that an attacker is actively intercepting communications and may be positioned to steal credentials, manipulate traffic, or deliver malicious content.

## Key Takeaways

- MITM attacks involve interception of communication.
- ARP spoofing can position an attacker between a victim and gateway.
- Duplicate IP-to-MAC mappings are a useful ARP spoofing indicator.
- Unexpected DNS responders can indicate DNS spoofing.
- Wireshark filters can help isolate suspicious network traffic.
- MITM findings should be investigated as potentially high-impact activity.

## Evidence

![MITM Detection Completion](../../../images/man-in-the-middle.png)

## Status

**Completed — 100%**
