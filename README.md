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

OPcap is an offline, read-only forensic analyzer for pcap and pcapng capture files. Built on the Python standard library, it reconstructs conversations and decodes link, network, transport and application protocols without replaying traffic. Findings are summarised with a weighted risk grade and MITRE ATT&CK references.

---

## ✨ Features

- Hand-written pcap/pcapng readers with decoders for IPv4/IPv6, TCP/UDP, DNS, HTTP, TLS and more
- Conversation table, top talkers, protocol hierarchy and port statistics
- Cleartext credential extraction from FTP, Telnet, HTTP, POP3, IMAP and SMTP
- Port-scan, host-sweep, beaconing/C2 and DGA/tunnelling heuristics
- ARP-spoofing detection and HTTP object carving
- Weighted A+ to F risk grade with severity filtering and multiple report formats

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OPcap -p capture.pcap --flows --dns --http
./OPcap -p capture.pcapng --modules all --format json -o report.json
./OPcap --demo --grade
./OPcap --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
