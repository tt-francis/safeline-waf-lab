# 🔐 SafeLine WAF Cybersecurity Lab

This project demonstrates a hands-on cybersecurity home lab featuring a Web Application Firewall (WAF) setup using **SafeLine**. The lab simulates a production-grade web application environment to practice network security, firewall configuration, and system hardening.

> 📸 Screenshots and walkthrough video coming soon!

---

## 📌 What This Project Covers

- Deployment of a Web Application Firewall using [SafeLine](https://www.safeline.io)
- Virtualization using VirtualBox
- Linux administration (Ubuntu + Kali)
- Apache Web Server setup
- Generating and installing SSL/TLS certificates using OpenSSL
- Manual traffic inspection and filtering
- Basic scripting & automation

---

## 🛠️ Tech Stack

| Component      | Description                         |
|----------------|-------------------------------------|
| VirtualBox     | Virtualization Platform             |
| Kali Linux     | Attacker / Testing Machine          |
| Ubuntu Server  | Host for Apache and SafeLine WAF    |
| Apache2        | Web server with HTTP/HTTPS support  |
| OpenSSL        | SSL Certificate generation          |
| SafeLine WAF   | Web Application Firewall            |

---

## 🧪 Lab Topology

```plaintext
┌────────────┐      HTTP/HTTPS      ┌────────────┐
│ Kali Linux │  <---------------->  │  SafeLine  │
│  (Attacker)│                      │    WAF     │
└────────────┘                      └────┬───────┘
                                        │
                                   ┌────▼──────┐
                                   │  Apache2  │
                                   │ Ubuntu VM │
                                   └───────────┘
