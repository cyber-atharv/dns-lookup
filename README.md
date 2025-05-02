# 🌐 DNS Reconnaissance & Lookup CLI

> A fast, interactive DNS querying and reconnaissance CLI tool built in Python for network discovery, WHOIS auditing, and security investigations.

[![Author](https://img.shields.io/badge/Made%20by-cyber--atharv-00ffcc?style=flat-square&logo=github)](https://github.com/cyber-atharv)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)

---

## 📌 What is DNS Reconnaissance?

The **Domain Name System (DNS)** is the phonebook of the Internet, translating human-friendly names (like `example.com`) into IP addresses. In cybersecurity, DNS reconnaissance is one of the initial steps of the reconnaissance phase. It reveals mail servers, subdomains, SPF/DKIM email verification records, and hosting providers.

This tool, created by **cyber-atharv**, provides an intuitive, formatted terminal tool for querying and analyzing DNS records with speed and clarity.

---

## ✨ Key Features

- **Comprehensive Record Queries:** Query `A` (IPv4), `AAAA` (IPv6), `MX` (Mail), `NS` (Name Servers), `TXT` (SPF/Verification), `CNAME` (Aliases), and `SOA` records.
- **Reverse DNS Lookups (`reverse`):** Query IP addresses to resolve their associated hostnames and PTR records.
- **DNS Resolution Tracer (`trace`):** Follow the query hierarchy starting from root nameservers down to authoritative domain nameservers.
- **Batch Processing (`batch`):** Query lists of domains concurrently to speed up penetration testing workflows.
- **WHOIS Domain Lookup:** Fetch domain registrar, expiry dates, and registration info.
- **Clean Terminal UI:** Uses Python Rich to present records in beautifully colored tables and JSON exports.

---

## 🚀 Quick Start & Usage

### 1. Installation
```bash
cd dns-lookup
pip install -e .
```

### 2. Examples

#### 🔹 Look up all DNS records for a domain
```bash
dnslookup query github.com
```

#### 🔹 Query specific record types (e.g. Mail & TXT records)
```bash
dnslookup query google.com --type MX
dnslookup query google.com --type TXT
```

#### 🔹 Reverse DNS lookup (IP to Hostname)
```bash
dnslookup reverse 8.8.8.8
# Output: dns.google
```

#### 🔹 Trace DNS resolution path
```bash
dnslookup trace cloudflare.com
```

---

## 🧠 Why I Built This

Standard command-line tools like `dig` and `nslookup` can have cluttered, raw outputs that are difficult to parse quickly during a security assessment. I built `dnslookup` to automate multi-record lookups, provide instant readable summaries with color coding, and allow fast JSON exports for custom security scripts.

---

## 📜 Author & License

- **Author:** [cyber-atharv](https://github.com/cyber-atharv)
- **License:** Open source under the MIT / AGPL License.
