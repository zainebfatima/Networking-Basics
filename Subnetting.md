# 🌐 Subnetting – Network Fundamentals Report

## 📌 Introduction
Subnetting is a fundamental concept in computer networking that involves dividing a large IP network into smaller, manageable sub-networks (subnets). It improves network performance, enhances security, and ensures efficient utilization of IP addresses.

---

## 🎯 Objectives
- Understand the concept of subnetting  
- Learn how to divide networks into smaller subnets  
- Improve IP address management  
- Reduce network congestion  

---

## 📖 What is Subnetting?
Subnetting is the process of splitting a large network into smaller networks using a subnet mask. Each subnet works independently while remaining part of the main network.

---

## 🔢 Key Concepts

### 1. IP Address
An IP address is a unique identifier assigned to each device on a network.

Example:192.168.1.1

### 2. Subnet Mask
A subnet mask determines which part of the IP address represents the network and which part represents the host.

Example:255.255.255.0

### 3. CIDR Notation
CIDR (Classless Inter-Domain Routing) is a compact way to represent subnet masks.

Example:192.168.1.0/24

---

## ⚙️ Why Subnetting is Important
- Efficient use of IP addresses  
- Improved network performance  
- Enhanced security  
- Easier network management  

---

## 🧮 Subnetting Example

### Given:
Network: `192.168.1.0/24`  
Required Subnets: `4`

### Step 1: Borrow Bits
2^2 = 4 → Borrow 2 bits

New Subnet Mask:
/26 → 255.255.255.192

### Step 2: Subnet Table

| Subnet | Network Address | Usable IP Range | Broadcast Address |
|--------|----------------|-----------------|------------------|
| 1 | 192.168.1.0 | 192.168.1.1 – 192.168.1.62 | 192.168.1.63 |
| 2 | 192.168.1.64 | 192.168.1.65 – 192.168.1.126 | 192.168.1.127 |
| 3 | 192.168.1.128 | 192.168.1.129 – 192.168.1.190 | 192.168.1.191 |
| 4 | 192.168.1.192 | 192.168.1.193 – 192.168.1.254 | 192.168.1.255 |

---

## 🛠️ Types of Subnetting

### Fixed Length Subnet Mask (FLSM)
- All subnets are equal in size  
- Easy to implement  
- Less efficient  

### Variable Length Subnet Mask (VLSM)
- Subnets can have different sizes  
- More efficient IP usage  
- More complex  

---

## 🚀 Advantages
- Better network performance  
- Reduced broadcast traffic  
- Improved security  
- Scalability  

---

## ⚠️ Disadvantages
- Requires proper planning  
- Can be complex for beginners  
- Misconfiguration may cause issues  

---

## 📚 Conclusion
Subnetting is an essential networking technique that improves efficiency, security, and performance of networks. Understanding subnetting is important for network design and management.

---

## 🔗 References
- RFC 950 – Internet Standard Subnetting Procedure  
- Cisco Networking Basics  
- Networking textbooks and online tutorials  
