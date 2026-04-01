# 🌐 ARP Tables – Networking Fundamentals Report

## 📌 Introduction
An **ARP table** (Address Resolution Protocol table) is a data structure maintained by a network device, such as a router or computer, that maps **IP addresses** to their corresponding **MAC addresses**. It helps devices communicate efficiently on a local area network (LAN) without repeatedly broadcasting ARP requests.

---

## 🎯 Objectives
- Understand the purpose of ARP tables  
- Learn how ARP tables are created and maintained  
- Explore how ARP tables improve network efficiency  
- Identify security considerations related to ARP tables  

---

## 📖 What is an ARP Table?
An **ARP table** stores the IP-to-MAC address mappings of devices that a network device has communicated with. By maintaining this table, the device can quickly forward data without sending an ARP broadcast for every packet.

---

## 🔢 Key Concepts

### 1. IP Address
- Logical identifier for a device  
- Used for routing packets in a network  

### 2. MAC Address
- Physical hardware address of a network interface  
- Unique to each network device  

---

## ⚙️ How ARP Tables Work
1. Device A wants to send data to Device B in the same LAN  
2. Device A checks its ARP table for Device B’s MAC address  
3. If an entry exists, Device A uses the MAC to send the packet directly  
4. If no entry exists, Device A sends an **ARP request** and waits for the **ARP reply**  
5. The new IP-MAC mapping is stored in the ARP table  

---

## 🛠️ Example of an ARP Table

| IP Address      | MAC Address        | Interface | Type    |
|-----------------|-----------------|-----------|---------|
| 192.168.1.2     | 00:1A:2B:3C:4D:5E | eth0      | Dynamic |
| 192.168.1.3     | 00:1A:2B:3C:4D:5F | eth0      | Dynamic |
| 192.168.1.1     | 00:1A:2B:3C:4D:60 | eth0      | Static  |

**Types of Entries:**
- **Dynamic:** Learned automatically via ARP requests  
- **Static:** Manually configured to prevent changes  

---

## 🚀 Advantages of ARP Tables
- Reduces network traffic by minimizing ARP broadcasts  
- Speeds up device-to-device communication  
- Provides a record of IP-to-MAC mappings for troubleshooting  

---

## ⚠️ Security Considerations
- ARP tables are vulnerable to **ARP spoofing / poisoning attacks**  
- Attackers can insert fake IP-MAC mappings to intercept network traffic  
- Regular monitoring and security measures like **static ARP entries** or **dynamic ARP inspection** are recommended  

---

## 📚 Conclusion
ARP tables are essential for efficient LAN communication, storing IP-to-MAC mappings to reduce unnecessary ARP broadcasts. Understanding ARP tables is crucial for network troubleshooting and security.

---

## 🔗 References
- RFC 826 – Ethernet Address Resolution Protocol  
- Cisco Networking Fundamentals  
- Networking textbooks and tutorials  
