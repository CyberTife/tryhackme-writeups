# 🔎 Phishing Analysis Fundamentals

## 📌 Overview

This TryHackMe room introduced the fundamental components of email
communication and the techniques used to analyze suspicious emails.

The room focused on understanding email addresses, email delivery,
email headers, email bodies, and different types of phishing attacks.

## 🎯 Objectives

The main objectives of this room were to:

- Understand the structure of an email
- Learn how emails are delivered
- Understand email headers
- Analyze email bodies
- Identify common phishing indicators
- Understand different types of phishing attacks

## 🧠 Key Concepts Learned

### 1. Email Addresses

I learned how email addresses are structured and why examining the
sender's address is important during phishing investigations.

Attackers may use:

- Lookalike domains
- Spoofed addresses
- Compromised accounts
- Slight variations of legitimate domains

These techniques can make malicious emails appear legitimate.

### 2. Email Delivery

I learned the basic process involved in email delivery and the role
of SMTP (Simple Mail Transfer Protocol) in transferring emails
between mail servers.

Understanding email delivery is useful when investigating the
origin and path of a suspicious email.

### 3. Email Headers

Email headers contain important technical information that can help
an analyst investigate a suspicious message.

Some important headers include:

- `From`
- `To`
- `Subject`
- `Date`
- `Reply-To`
- `Received`
- `Message-ID`

The `Received` headers can provide useful information about the
servers involved in delivering an email.

### 4. Email Body Analysis

The email body can contain several indicators of a phishing attempt.

During the room, I learned to look for:

- Suspicious links
- Unexpected attachments
- Urgent language
- Requests for credentials
- Requests for financial information
- Impersonation
- Social engineering techniques

### 5. Types of Phishing

I learned about different phishing techniques and how attackers
use social engineering to manipulate victims.

Examples include:

- Phishing
- Spear phishing
- Whaling
- Smishing
- Vishing

## 🔐 SOC Analyst Relevance

Phishing is a common initial access technique used by attackers.

As a SOC Analyst, analyzing suspicious emails can involve:

1. Reviewing the sender and recipient information
2. Examining email headers
3. Inspecting URLs and attachments
4. Identifying Indicators of Compromise (IOCs)
5. Determining whether the email is malicious
6. Assessing the potential impact
7. Escalating or responding to the incident

This room helped me understand how email analysis contributes to
threat detection and incident response.

## 🛠️ Platform

- TryHackMe

## 📚 Skills Practiced

- Phishing Analysis
- Email Analysis
- Email Header Analysis
- Social Engineering Detection
- IOC Identification
- Threat Detection
- Incident Response Fundamentals

## 💡 Key Takeaway

My biggest takeaway from this room is that phishing analysis goes
beyond simply looking at whether an email "looks suspicious."

A SOC Analyst needs to examine the technical and contextual evidence
within the email and use multiple indicators to determine whether
the message is legitimate or malicious.

## 📸 Room Completion

The room was completed successfully.

![Phishing Analysis Fundamentals - Completed](./screenshots/room-completed.png)

## ✅ Status

**Completed — 100%**
