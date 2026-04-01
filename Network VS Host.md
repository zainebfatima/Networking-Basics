# 🌐 Network vs Hosts – Networking Fundamentals Report

## 📌 Introduction
In computer networking, every IP address consists of two main parts: the **Network** portion and the **Host** portion. Understanding the difference between network and host is essential for designing, managing, and troubleshooting networks.

---

## 🎯 Objectives
- Understand the difference between network and host addresses  
- Learn how to identify network and host portions in an IP address  
- Calculate usable host addresses in a subnet  
- Understand the role of subnet masks  

---

## 📖 Key Concepts

### 1. IP Address
An IP address is a unique identifier for a device on a network.  
Example:192.168.1.10

### 2. Network Portion
The **network portion** identifies the specific network to which a device belongs.  
- Determined by the subnet mask  
- Same for all devices in the same network  

Example:IP: 192.168.1.10
Subnet Mask: 255.255.255.0
Network Address: 192.168.1.0

### 3. Host Portion
The **host portion** identifies the specific device within the network.  
- Varies for each device in the network  
- Determines the unique address of a device  

Example:Host ID: 10

---

## ⚙️ How to Determine Network vs Host

### Step 1: Identify Subnet Mask
Subnet Mask: 255.255.255.0 → /24

### Step 2: Network Bits vs Host Bits
Network Bits = 24
Host Bits = 32 - 24 = 8

### Step 3: Calculate Network Address
- Perform **bitwise AND** between IP and subnet mask:
- 192.168.1.10 AND 255.255.255.0 = 192.168.1.0
- 
### Step 4: Identify Usable Hosts
Usable Hosts = 2^(Host Bits) - 2 = 2^8 - 2 = 254

---

## 🧮 Example Table

| IP Address       | Subnet Mask       | Network Address | Usable Hosts      |
|-----------------|-----------------|----------------|-----------------|
| 192.168.1.10    | 255.255.255.0    | 192.168.1.0    | 192.168.1.1 – 192.168.1.254 |
| 10.0.5.20       | 255.255.255.192  | 10.0.5.0       | 10.0.5.1 – 10.0.5.62         |

---

## 🚀 Summary
- **Network portion** identifies the network  
- **Host portion** identifies the device within the network  
- Subnet mask divides the IP address into network and host  
- Proper understanding helps in subnetting, IP management, and network troubleshooting  

---

## 🔗 References
- Cisco Networking Basics  
- RFC 950 – Internet Standard Subnetting Procedure  
- Networking textbooks and online tutorials  
