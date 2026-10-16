# 🦉 OPcap

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OPcap** — Offline PCAP Forensic Analyzer

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Offline PCAP/PCAPNG forensic analyzer — flows, creds, DNS, TLS, threats

---

## ✨ Features

- Hand-written pcap reader (LE/BE, usec/nsec magic) and pcapng reader (SHB / IDB / EPB / SPB / OPB)
- Link layers: Ethernet, 802.1Q/QinQ, Linux SLL/SLL2, BSD loopback/NULL, raw IPv4/IPv6
- Decoders: IPv4, IPv6 (+ext headers), TCP, UDP, ICMP/ICMPv6, ARP
- App decoders: DNS, HTTP, DHCP, FTP, Telnet, SMTP, POP3, IMAP, TLS ClientHello (SNI, ALPN, JA3)
- Conversation table, top talkers, protocol hierarchy, port statistics, DNS log, HTTP log
- Cleartext credential extraction (FTP / Telnet / HTTP Basic / HTTP forms / POP3 / IMAP / SMTP AUTH)
- Port-scan & host-sweep detection, beaconing / C2 heuristics, DGA / tunnelling DNS heuristics, ARP spoofing detection
- HTTP object carving (Content-Length / chunked)
- Weighted A+…F risk grade, MITRE ATT&CK tags, remediation guidance
- Export TXT / MD / JSON / CSV / SARIF
- --demo: synthesise a sample capture & self-test
- Strictly offline & read-only — never captures traffic

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OPcap
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
