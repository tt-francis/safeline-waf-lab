#  SafeLine WAF Cybersecurity Lab

This project demonstrates a hands-on cybersecurity home lab featuring a Web Application Firewall (WAF) setup using **SafeLine**. The lab simulates a production-grade web application environment to practice network security, firewall configuration, and system hardening.

> 📸 Screenshots and walkthrough video coming soon!
>
> Mastercard Cybersecurity virtual experience program on Forage - April 2025


 * Completed a job simulation where I served as an analyst on Mastercard’s
   Security Awareness Team 
 * Helped identify and report security threats such as phishing 
 * Analyzed and identified which areas of the business needed more robust
   security training and implemented training courses and procedures for those
   teams

---

## What This Project Covers

- Deployment of a Web Application Firewall using [SafeLine](https://www.safeline.io)
- Virtualization using VirtualBox
- Linux administration (Ubuntu + Kali)
- Apache Web Server setup
- Generating and installing SSL/TLS certificates using OpenSSL
- Manual traffic inspection and filtering
- Basic scripting & automation

---

## Tech Stack

| Component      | Description                         |
|----------------|-------------------------------------|
| VirtualBox     | Virtualization Platform             |
| Kali Linux     | Attacker / Testing Machine          |
| Ubuntu Server  | Host for Apache and SafeLine WAF    |
| Apache2        | Web server with HTTP/HTTPS support  |
| OpenSSL        | SSL Certificate generation          |
| SafeLine WAF   | Web Application Firewall            |

---

## Lab Topology

```markdown
┌────────────┐      HTTP/HTTPS      ┌────────────┐
│ Kali Linux │  <---------------->  │  SafeLine  │
│  (Attacker)│                      │    WAF     │
└────────────┘                      └────┬───────┘
                                        │
                                   ┌────▼──────┐
                                   │  Apache2  │
                                   │ Ubuntu VM │
                                   └───────────┘
```

---

## How I Set It Up

1. Created two VMs in VirtualBox: one Kali Linux, one Ubuntu Server.
2. Installed Apache on Ubuntu to host a demo investment website.
3. Generated SSL certificates with OpenSSL and configured HTTPS.
4. Installed and configured SafeLine WAF in reverse proxy mode.
5. Simulated attacks from Kali to test WAF detection and logging.
6. Tuned WAF rules, reviewed logs, and refined response policies.

---

## Learning Outcomes

- Configuring and testing real-world WAFs in a safe lab.
- Gained hands-on experience with HTTPS, reverse proxies, and traffic filtering.
- Practical skills in scripting, Linux troubleshooting, and web server management.
- Better understanding of attack simulation and blue team operations.

---

## 🚧 Next Steps

- ✅ Record walkthrough demo
- ✅ Upload screenshots from both VMs
- ⏳ Add automated BASH or Python setup script
- ⏳ Extend WAF rules for custom detections




