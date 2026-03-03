# Ports Basics

## What is a Port?

- Port is a number that identifies a **specific service/program** on a computer  
- IP = building address, Port = apartment number  

Example:  
- Browser connects to a web server → port 443 (HTTPS)  
- Email client sends emails → port 25 (SMTP)  

---

## Total Ports

- 0 – 65535 ports  
- Well-known: 0–1023  
- Registered: 1024–49151  
- Dynamic/Private: 49152–65535  

---

## TCP vs UDP

| Protocol | Feature | Example |
|----------|--------|--------|
| TCP      | Reliable, ensures delivery | HTTP, HTTPS, SSH |
| UDP      | Fast, not guaranteed delivery | DNS, Online gaming, Streaming |

---

## Local vs Foreign Address

- **Local Address** → Your computer IP + port  
- **Foreign Address** → Remote computer IP + port  
- Shows “who is talking to whom”
- # Lab: Check Open Ports on Your Computer

### Windows
1. Press `Win + R` → type `cmd` → Enter  
2. Type `netstat -an` → Enter  
3. Look at Local Address, Foreign Address, and State  

### Linux / Mac
1. Open Terminal  
2. Type `netstat -an` or `ss -tuln`  
3. Observe open/listening ports  

**Observation**:  
- LISTENING → waiting for incoming connections  
- ESTABLISHED → active connection  
- Check which services use which ports
