
# NetworkMiner

## Overview

This TryHackMe room introduced NetworkMiner and its use in network forensic analysis.

NetworkMiner is an open-source Network Forensic Analysis Tool (NFAT) that can analyse live traffic and captured PCAP files. It can provide a quick overview of hosts, sessions, protocols, credentials, files, parameters, keywords and other information extracted from network traffic.

## Learning Objectives

- Understand what NetworkMiner is
- Learn how NetworkMiner is used in network forensics
- Analyse captured network traffic
- Identify hosts and sessions
- Extract files and other information from PCAP files
- Investigate credentials, keywords, messages and anomalies

## What I Learned

### 1. NetworkMiner in Network Forensics

I learned that network forensics focuses on analysing network traffic to detect malicious activity, security breaches and network anomalies.

NetworkMiner can provide useful information about:

- Captured hosts
- IP and MAC addresses
- Hostnames
- Operating system information
- Open ports
- Potential attack indicators
- Network sessions
- Tools or toolkits used during attacks

### 2. Supported Data Types

I learned that network forensics can involve three main types of data:

- Live Traffic
- Traffic Captures
- Log Files

NetworkMiner can process live traffic and captured traffic, with PCAP analysis being one of its main uses.

### 3. NetworkMiner Capabilities

NetworkMiner provides several useful capabilities for network forensic investigations, including:

- Traffic sniffing
- PCAP parsing
- Protocol analysis
- OS fingerprinting
- File extraction
- Credential discovery
- Clear-text keyword parsing

These capabilities allow an analyst to quickly obtain useful information from captured network traffic.

### 4. Operating Modes

I learned about two main ways NetworkMiner can be used:

**Sniffer Mode**

NetworkMiner has a traffic sniffing capability, although the room explains that it is not intended to be used as a primary network sniffer.

**Packet Parsing/Processing**

NetworkMiner can process PCAP files and provide a quick overview of the captured traffic.

This makes it useful for finding the "low hanging fruit" before performing a deeper investigation with tools such as Wireshark.

### 5. NetworkMiner vs Wireshark

One of the important lessons was understanding the different purposes of NetworkMiner and Wireshark.

NetworkMiner is useful for quickly obtaining an overview of a PCAP and extracting useful information.

Wireshark is better suited for detailed packet-level investigation, protocol analysis, filtering and payload analysis.

A practical workflow is to use NetworkMiner for an initial overview and then use Wireshark for deeper investigation.

### 6. Hosts

The Hosts section provides information about identified hosts in the captured traffic.

Information can include:

- IP address
- MAC address
- Operating system
- Open ports
- Sent and received packets
- Incoming and outgoing sessions
- Host details

OS fingerprinting uses Satori and p0f information, while MAC address information can be resolved using a manufacturer database.

### 7. Sessions

The Sessions section displays detected sessions from the PCAP.

It can provide information such as:

- Frame number
- Client and server addresses
- Source and destination ports
- Protocol
- Start time

The filtering functionality can also be used to search for keywords within sessions.

### 8. DNS

The DNS section displays DNS queries and related information.

This can include:

- Frame number
- Timestamp
- Client and server
- Source and destination ports
- IP TTL
- DNS time
- Transaction ID
- Query type
- DNS query and answer

This can help analysts investigate DNS activity within a captured traffic file.

### 9. Credentials

NetworkMiner can extract credentials and password hashes from supported traffic.

Examples include:

- Kerberos hashes
- NTLM hashes
- RDP cookies
- HTTP cookies
- HTTP requests
- IMAP
- FTP
- SMTP
- MS SQL

This can be valuable during forensic investigations, especially when analysing traffic that contains authentication information.

### 10. Files and Images

NetworkMiner can identify and extract files transferred through captured traffic.

The Files section can provide information such as:

- Filename
- Extension
- File size
- Source and destination addresses
- Source and destination ports
- Protocol
- Timestamp
- Reconstructed path

The Images section can also display images extracted from the captured traffic.

### 11. Parameters and Keywords

NetworkMiner can identify parameters contained within captured traffic.

The Parameters section can provide:

- Parameter name
- Parameter value
- Frame number
- Source and destination hosts
- Source and destination ports
- Timestamp

The Keywords section can be used to search processed PCAP files for specific clear-text keywords and strings.

### 12. Messages

The Messages section can display extracted emails, chats and messages from captured traffic.

Information can include:

- Sender
- Receiver
- Source and destination hosts
- Protocol
- Timestamp
- Message size

Attachments and additional attributes can also be investigated when available.

### 13. Anomalies

NetworkMiner includes an Anomalies section that can display detected anomalies.

The room explains that NetworkMiner is not an IDS, but it includes detections for certain activities such as:

- EternalBlue exploitation
- Spoofing attempts

These detections can provide useful leads during a network forensic investigation.

### 14. Version Differences

I also learned that different NetworkMiner versions provide different features.

The room compared versions 1.6 and 2.7 and highlighted differences involving:

- MAC address processing
- Frame processing
- Parameter processing
- Clear-text data processing

This showed me that tool versions can affect the type and amount of information available during an investigation.

## Practical Skills

During this room, I practised and learned how to:

- Analyse PCAP files with NetworkMiner
- Identify hosts
- Investigate network sessions
- Review DNS activity
- Identify extracted credentials
- Extract files and images
- Investigate parameters
- Search for keywords
- Review messages
- Identify potential anomalies
- Use NetworkMiner for initial network forensic analysis

## Security Relevance

NetworkMiner can help a SOC analyst quickly understand what is happening within a captured network traffic file.

It can provide useful investigative leads such as communicating hosts, operating systems, open ports, credentials, transferred files, DNS activity and potential anomalies.

This makes it useful as an initial analysis tool before performing deeper packet-level investigation with Wireshark.

## Key Takeaways

The main lesson from this room was that NetworkMiner is particularly useful for quickly obtaining an overview of network traffic and extracting useful information from PCAP files.

I learned that NetworkMiner and Wireshark complement each other:

- **NetworkMiner:** Quick overview, host identification and data extraction
- **Wireshark:** Detailed packet analysis, filtering and protocol investigation

Using both tools together can make network forensic investigations more efficient.

## Completion

I completed the NetworkMiner room on TryHackMe.

## Platform

TryHackMe

## Skills Practised

NetworkMiner  
Network Forensics  
PCAP Analysis  
Network Traffic Analysis  
OS Fingerprinting  
Host Identification  
Session Analysis  
DNS Analysis  
Credential Discovery  
File Extraction  
Keyword Analysis  
Anomaly Detection

## Completion Evidence

![TryHackMe NetworkMiner Completion](networkminer-completion.png)
