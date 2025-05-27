# 🌐 Networking Basics Cheat Sheet

## 🧱 OSI Model - 7 Layers

| Layer | Name             | Function (Short)                        | Common Protocols/Examples |
|-------|------------------|------------------------------------------|----------------------------|
| 7     | Application      | User-facing applications                 | HTTP, FTP, DNS, SMTP       |
| 6     | Presentation     | Data formatting, encryption/decryption   | SSL, TLS, JPEG, ASCII      |
| 5     | Session          | Session setup, maintenance, teardown     | NetBIOS, RPC               |
| 4     | Transport        | Reliable delivery & flow control         | TCP, UDP                   |
| 3     | Network          | Routing & addressing                     | IP, ICMP, IPSec            |
| 2     | Data Link        | MAC address, frame delivery              | Ethernet, ARP, PPP         |
| 1     | Physical         | Hardware transmission of raw data        | Cables, NIC, Hubs          |

💡 Mnemonic: **All People Seem To Need Data Processing**

---

## 📦 Common Protocols and Their Ports

| Protocol      | Port | Description                               |
|---------------|------|-------------------------------------------|
| HTTP          | 80   | Web browsing (insecure)                   |
| HTTPS         | 443  | Secure web browsing                       |
| FTP           | 21   | File transfer protocol                    |
| SSH           | 22   | Secure shell (remote login)               |
| Telnet        | 23   | Remote login (insecure)                   |
| DNS           | 53   | Domain Name System                        |
| DHCP          | 67/68| Dynamic Host Configuration Protocol       |
| SMTP          | 25   | Email sending                             |
| POP3          | 110  | Email retrieval                           |
| IMAP          | 143  | Email access                              |
| RDP           | 3389 | Remote Desktop Protocol                   |
| SNMP          | 161  | Network device management                 |
| ICMP          | -    | Used by ping/traceroute (Layer 3 protocol)|
| NTP           | 123  | Network Time Protocol                     |

---

## 📘 CIDR Notation (Quick Reference)

CIDR defines how many bits are used for the **network portion** of an IP address.

| CIDR  | Subnet Mask       | IPs in Range | Usable IPs |
|-------|-------------------|--------------|------------|
| /8    | 255.0.0.0         | ~16.7M       | 16,777,214 |
| /16   | 255.255.0.0       | 65,536       | 65,534     |
| /24   | 255.255.255.0     | 256          | 254        |
| /30   | 255.255.255.252   | 4            | 2          |

🧠 *Usable IPs = Total - 2 (Network & Broadcast IPs)*

---

## 🔗 IP Address Types

- **Private IPs (for internal use):**
  - Class A: 10.0.0.0 – 10.255.255.255
  - Class B: 172.16.0.0 – 172.31.255.255
  - Class C: 192.168.0.0 – 192.168.255.255

- **Public IPs** are globally routable and assigned by ISPs.

---

## 🧠 Interview-Style Quick Q&A

**Q: What is the OSI Model?**  
A: A 7-layer architecture to standardize network communication.

**Q: What's the difference between TCP and UDP?**  
A: TCP is connection-oriented and reliable; UDP is faster but connectionless and less reliable.

**Q: How do you identify a private IP?**  
A: Check if it falls within the reserved private ranges.

**Q: What is CIDR?**  
A: Classless Inter-Domain Routing — it determines how many bits are used for network in an IP.

---

✅ *Perfect for DevOps, Cloud, Sysadmin & Interview Prep!*
