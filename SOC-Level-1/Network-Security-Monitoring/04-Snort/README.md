# Snort

## Overview

This lab provided hands-on experience with Snort, an open-source intrusion detection solution, including Snort modes, rule creation, real-time detection, and PCAP analysis.

## What I Learned

I learned that Snort can be used for network monitoring, packet logging, and intrusion detection. Its NIDS functionality applies rules to network traffic and generates alerts when traffic matches a detection rule.

## Snort Modes

### Packet Sniffer Mode

Displays network packets without performing intrusion analysis. It can be useful for troubleshooting and understanding traffic flows.

### Packet Logging Mode

Records network traffic into PCAP files for later analysis and forensic investigation.

### NIDS Mode

Monitors traffic in real time, applies detection rules, and generates alerts when a rule matches.

## Snort Rule Structure

A Snort rule contains important fields such as:

- Action
- Protocol
- Source IP
- Source port
- Direction
- Destination IP
- Destination port
- Message
- Signature ID (SID)
- Revision number

Example:

```text
alert icmp any any -> 127.0.0.1 any (msg:"Loopback Ping Detected"; sid:10003; rev:1;)
```

This rule generates an alert when ICMP traffic is detected toward the loopback address.

## Practical Exercise

I created a custom Snort rule and tested it by generating ICMP traffic with:

```bash
ping 127.0.0.1
```

Snort successfully generated an alert confirming that the rule worked.

I also learned how Snort can analyze previously captured network traffic using PCAP files, which is useful during forensic investigations.

## SOC Relevance

Snort is relevant to SOC work because it can provide network-based detection alerts. Analysts can use those alerts as an investigation starting point and correlate them with other telemetry to determine severity and impact.

## Key Takeaways

- Snort can sniff, log, and detect network traffic.
- Snort rules define what activity should trigger an alert.
- `sid` identifies a rule.
- `rev` tracks rule revisions.
- PCAP analysis can support forensic investigations.
- Custom rules can be created for specific detection requirements.

## Evidence

![Snort Completion](../../../images/snort.png)

## Status

**Completed — 100%**
