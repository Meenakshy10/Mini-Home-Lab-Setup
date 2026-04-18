🏠 Cybersecurity Home Lab Setup

## 📌 Overview

Built a personal cybersecurity home lab from scratch to simulate real-world attack and defense scenarios in a completely safe and isolated environment. This lab serves as the foundation for all SOC analyst projects in this portfolio.

The goal of this lab is to practice skills that a real SOC Analyst uses daily — including attack simulation, log monitoring, SIEM configuration, and incident detection.

---

## 🖥️ Lab Architecture

| Component          | Details                          |
|--------------------|----------------------------------|
| Host Machine       | Windows 11 (Physical Laptop)     |
| Virtualization     | Oracle VirtualBox                |
| Attacker Machine   | Kali Linux 2026.1 (VM)           |
| Target Machine     | Windows 10 (VM)                  |
| Network Type       | Bridged Adapter                  |
| Kali IP Address    | 192.168.0.132                    |
| Windows IP Address | 192.168.0.130                    |
| Connectivity       | Verified ✅ (Ping successful)   |

---

## 🎯 Purpose of This Lab

This home lab was built to practice and demonstrate the following real-world SOC analyst skills:

- **Attack Simulation** — Using Kali Linux to simulate brute force and network attacks against Windows target
- **Log Monitoring** — Collecting and analyzing Windows and Linux system logs
- **SIEM Configuration** — Installing and configuring Wazuh SIEM for threat detection
- **Incident Detection** — Creating custom alert rules and monitoring dashboards
- **Network Analysis** — Capturing and analyzing network traffic using Wireshark
- **Vulnerability Assessment** — Scanning and identifying vulnerabilities using Nmap

---

## 🔧 Tools Installed

| Tool            | Machine      | Purpose                           |
|-----------------|--------------|-----------------------------------|
| Kali Linux      | Attacker VM  | Penetration testing platform      |
| Hydra           | Kali VM      | Brute force attack simulation     |
| Nmap            | Kali VM      | Network scanning & enumeration    |
| Wireshark       | Kali VM      | Packet capture and analysis       |
| Metasploit      | Kali VM      | Exploitation framework            |
| Windows 10      | Target VM    | Target machine for simulations    |
| Wazuh Agent     | Windows VM   | Log collection and forwarding     |

---

## 🌐 Network Setup

```
┌──────────────────────┐        Bridged Network         ┌──────────────────────┐
│                      │                                 │                      │
│   Kali Linux VM      │◄───────────────────────────────│   Windows 10 VM      │
│   (Attacker)         │     ping successful ✅          │   (Target)           │
│   192.168.0.132      │                                 │   192.168.0.130      │
└──────────────────────┘                                 └──────────────────────┘
```

Both machines are connected via Bridged Adapter — allowing full communication between the attacker and target machines for realistic attack simulation!

---

## ✅ Connectivity Proof

Successful ping from Kali Linux to Windows 10 VM confirmed:

```
PING 192.168.0.130 (192.168.0.130) 56(84) bytes of data.
64 bytes from 192.168.0.130: icmp_seq=1 ttl=128 time=4.75 ms
64 bytes from 192.168.0.130: icmp_seq=2 ttl=128 time=3.58 ms
64 bytes from 192.168.0.130: icmp_seq=3 ttl=128 time=3.32 ms
```

---

## 📸 Screenshots

| File | Description |
|------|-------------|
| 01-kali-desktop.png | Kali Linux VM running |
| 02-windows-desktop.png | Windows 10 VM running |
| 03-kali-ip.png | Kali Linux IP configuration (ip a) |
| 04-windows-ip.png | Windows 10 IP configuration (ipconfig) |
| 05-kali-ping-windows.png | Successful ping from Kali to Windows ✅ |

---

## 🔗 Projects Built Using This Lab

| # | Project Name | Tools Used | Status |
|---|---|---|---|
| 1 | Phishing Email Investigation | VirusTotal, MXToolbox, Whois | ✅ Completed |
| 2 | Brute Force Attack Detection | Hydra, Wazuh, Windows Logs | 🔜 In Progress |
| 3 | SOC Monitoring Lab with Wazuh | Wazuh SIEM, Windows Logs | ⏳ Upcoming |
| 4 | Network Traffic Analysis | Wireshark, PCAP files | ⏳ Upcoming |
| 5 | SIEM Dashboard + Alert Rules | Splunk / Wazuh | ⏳ Upcoming |
| 6 | Vulnerability Assessment | Nmap, OpenVAS | ⏳ Upcoming |
| 7 | Incident Response + MITRE ATT&CK | MITRE ATT&CK Framework | ⏳ Upcoming |
| 8 | Log Analysis & Threat Hunting | Log files, analysis tools | ⏳ Upcoming |

---

## ⚠️ Disclaimer

This home lab is built purely for **educational purposes**.
All attacks and simulations are performed within a **controlled virtual environment** on machines I personally own.
No external or real-world systems were targeted or harmed.

---

## 👩‍💻 About

**[MEENAKSHY B R]**
Cybersecurity Enthusiast | Aspiring SOC Analyst

