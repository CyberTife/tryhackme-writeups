# Wireshark: The Basics

## Overview

This TryHackMe room introduced the fundamentals of Wireshark and packet analysis.

Wireshark is an open-source, cross-platform network packet analyser used to capture, inspect and investigate network traffic and PCAP files.

## Learning Objectives

- Navigate and configure Wireshark
- Inspect packets across different TCP/IP layers
- Understand packet dissection
- Analyse network traffic
- Apply display filters
- Follow network streams
- Extract files and objects from packet captures
- Use Wireshark's Expert Information

## What I Learned

### 1. Wireshark Interface

I learned how to navigate the main Wireshark interface, including:

- Toolbar
- Display Filter Bar
- Packet List Pane
- Packet Details Panel
- Packet Bytes Pane
- Status Bar
- Capture interfaces

### 2. PCAP Analysis

I learned how to open and investigate `.pcap` and `.pcapng` files.

The packet list provides a summary of captured traffic, while the packet details and packet bytes panes allow deeper investigation of individual packets.

### 3. Packet Dissection

Wireshark breaks packets down into different protocol layers.

I learned to identify:

- Frame information
- MAC addresses
- IPv4 addresses
- TCP/UDP information
- Source and destination ports
- Application protocols
- Application data

### 4. Packet Filtering

I practised using display filters to reduce the amount of traffic being investigated.

Examples include:

```text
http
tcp.port == 80
ip.addr == 10.10.10.111
http.request.method == "GET"
dns
```
### 5. Following Network Streams

I learned how to follow TCP, UDP and HTTP streams to reconstruct application-level communication.

This can help analysts investigate information such as:

- HTTP requests and responses
- User activity
- Transferred data
- Clear-text credentials
- Suspicious communications

### 6. Exporting Objects

Wireshark can extract files transferred through supported protocols.

This is useful during network investigations because analysts can extract suspicious files and investigate them separately.

### 7. Expert Information

I learned that Wireshark provides Expert Information to highlight possible protocol problems and unusual events.

The severity categories include:

- Chat
- Note
- Warn
- Error

Expert Information is useful for identifying potential anomalies, although it should be treated as an investigative aid rather than definitive proof of malicious activity.

## Practical Skills

During this room, I practised:

- Opening PCAP files
- Navigating packet captures
- Inspecting packet layers
- Identifying network protocols
- Filtering traffic
- Following network streams
- Extracting objects
- Investigating packet metadata
- Using Expert Information

## Security Relevance

Packet analysis is an important skill for a SOC analyst.

Wireshark can help analysts investigate suspicious network behaviour, identify unusual communications, inspect protocols and understand what happened during a security event.

## Key Takeaways

The main lesson from this room was that effective packet analysis requires understanding both the network protocols and the information contained within individual packets.

Wireshark provides the visibility needed to move from a high-level view of network traffic to detailed packet-level investigation.

## Completion

I completed the Wireshark: The Basics room on TryHackMe.

## Platform

TryHackMe

## Skills Practised

Wireshark PCAP Analysis Packet Analysis Network Forensics TCP/IP HTTP DNS Display Filters
