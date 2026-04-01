# 🌐 ARP Protocol – Networking Fundamentals Report

## 📌 Introduction
ARP (Address Resolution Protocol) is a network protocol used to map a device’s **IP address** to its **MAC (hardware) address** on a local area network (LAN). It is an essential protocol for network communication in IPv4 networks.

---

## 🎯 Objectives
- Understand what ARP is and why it is important  
- Learn how ARP resolves IP addresses to MAC addresses  
- Explore ARP types and working  
- Identify security concerns related to ARP  

---

## 📖 What is ARP?
ARP stands for **Address Resolution Protocol**. It operates at the **Data Link Layer (Layer 2)** and is used by devices to discover the MAC address corresponding to an IP address. Without ARP, devices cannot communicate within the same network.

---

## 🔢 Key Concepts

### 1. IP Address
- Logical address assigned to a device  
- Used for routing packets  

### 2. MAC Address
- Physical hardware address of a network interface  
- Unique for each network device  

---

## ⚙️ How ARP Works
1. Device A wants to send data to Device B on the same network  
2. Device A knows Device B’s IP but not its MAC  
3. Device A broadcasts an **ARP Request**: “Who has IP 192.168.1.10?”  
4. Device B responds with an **ARP Reply** containing its MAC address  
5. Device A caches the MAC in the **ARP table** and sends data  

---

## 🛠️ ARP Table
Each device maintains an ARP table to reduce repeated ARP requests.  

**Example ARP Table:**

| IP Address      | MAC Address        | Interface |
|-----------------|-----------------|-----------|
| 192.168.1.10    | 00:1A:2B:3C:4D:5E | eth0      |
| 192.168.1.11    | 00:1A:2B:3C:4D:5F | eth0      |

---

## 🧮 Types of ARP

### 1. Gratuitous ARP
- Sent by a device to **announce its IP-MAC mapping**  
- Useful for detecting IP conflicts  

### 2. Proxy ARP
- A router answers ARP requests on behalf of another device  
- Helps devices communicate across different subnets  

### 3. Reverse ARP (RARP)
- Used by a device to **discover its IP address** when it only knows its MAC  
- Mostly obsolete, replaced by DHCP  

---

## 🚀 Advantages
- Allows communication between devices on the same LAN  
- Maintains a cache to reduce network traffic  
- Simple and automatic IP-to-MAC resolution  

---

## ⚠️ Disadvantages / Security Issues
- ARP is **stateless and insecure**  
- Vulnerable to **ARP spoofing / ARP poisoning attacks**  
- Can lead to **man-in-the-middle attacks** if exploited  

---

## 📚 Conclusion
ARP is a critical protocol in networking that enables devices to map IP addresses to MAC addresses. While simple and effective, it has security risks that require careful network management.

---

## 🔗 References
- RFC 826 – Ethernet Address Resolution Protocol  
- Cisco Networking Academy  
- Networking textbooks and online tutorials  
