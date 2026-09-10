# Data Exfiltration Detection

## Overview

This lab focused on detecting attempts to move sensitive data outside an organization using network protocols such as DNS, FTP, and HTTP.

## What I Learned

I learned that data exfiltration can occur after an attacker gains access to a system and collects valuable information. The attacker may stage, compress, encode, encrypt, and then transfer the data through different network channels.

Detection is more effective when network, host, and cloud telemetry are correlated instead of relying on one alert.

## DNS Exfiltration / DNS Tunneling

DNS is attractive to attackers because DNS traffic is common and normally allowed through many network controls. Attackers can encode data inside DNS queries or responses, particularly within subdomain labels or TXT records.

### Indicators

- Many DNS queries sent to one external domain
- Very long subdomain/query names
- High-entropy or Base32/Base64-like strings
- Unusual TXT or NULL records
- Frequent NXDOMAIN responses
- Regular query intervals that may indicate beaconing

### Wireshark Filters

```text
dns
```

```text
dns.flags.response == 0
```

```text
dns && frame.len > 70
```

## FTP Exfiltration

Attackers can use FTP to move large amounts of data outside the network, including by abusing compromised credentials or legitimate FTP infrastructure.

Important indicators include `USER` and `PASS` commands, repeated `STOR` or `RETR` activity, large transfers to unusual external IPs, transfers outside normal business hours, and large payloads over FTP data channels.

## HTTP Exfiltration

HTTP can be abused because it blends into normal web traffic. Attackers may use large POST requests, encoded data in GET requests, custom headers, chunked or multipart transfers, HTTPS/TLS tunneling, or legitimate cloud services for staging.

### HTTP Indicators

- Unusually large HTTP POST requests
- Rare or low-reputation destinations
- Repeated small requests followed by a large upload
- Chunked or multipart transfers

A Splunk search used in the lab was:

```text
index="data_exfil" sourcetype="http_logs"
```

## Host and Cloud Indicators

Data exfiltration can also leave evidence on the endpoint or in cloud services. Examples include PowerShell/Invoke-WebRequest, `curl`/`wget`, `rclone`, `awscli`, archive creation, removable-media activity, cloud storage uploads, and external file sharing.

## SOC Investigation Approach

I learned that a strong investigation should answer:

1. What data was accessed?
2. Which user or process accessed it?
3. Was the data staged or compressed?
4. What destination received the data?
5. Which protocol was used?
6. How much data was transferred?
7. Is the destination known or suspicious?
8. What other alerts occurred before or after the transfer?

## SOC Relevance

Data exfiltration detection is directly relevant to SOC work because analysts must identify potential data breaches and determine whether sensitive information was transferred outside the organization.

The key lesson was that a single large outbound connection may not be enough to confirm exfiltration. Correlation across network, endpoint, DNS, authentication, and cloud logs provides stronger evidence.

## Key Takeaways

- Data exfiltration is the unauthorized movement of sensitive information out of an organization.
- Attackers can abuse normal protocols such as DNS, FTP, and HTTP.
- Large outbound traffic and unusual destinations are important investigation clues.
- Encoding, encryption, chunking, and low-and-slow techniques can make detection harder.
- Correlation across multiple telemetry sources improves detection accuracy.

## Evidence

![Data Exfiltration Detection Completion](../../../images/data-exfiltration.png)

## Status

**Completed — 100%**
