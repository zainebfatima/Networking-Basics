# 🌐 Network Address Translation (NAT) – Report

## 📌 Introduction
Network Address Translation (NAT) is a networking technique used to modify IP address information in packet headers while they are in transit. It allows multiple devices on a private network to share a single public IP address to access the internet.

---

## 🎯 Objectives
- Understand the concept of NAT  
- Learn how private and public IP addresses work  
- Explore types of NAT  
- Understand its advantages and limitations  

---

## 📖 What is NAT?
NAT (Network Address Translation) is a method used by routers to translate private IP addresses into a public IP address before sending data to the internet. When responses return, NAT converts the public IP back to the private IP of the device.

---

## 🔢 Key Concepts

### 1. Private IP Address
Used within a local network and not accessible directly from the internet.

Examples:
192.168.x.x
10.x.x.x
172.16.x.x – 172.31.x.x

---

### 2. Public IP Address
A globally unique IP address assigned by an Internet Service Provider (ISP) used to communicate over the internet.

---

### 3. NAT Table
A table maintained by the router that keeps track of translations between private and public IP addresses.

---

## ⚙️ How NAT Works
1. A device in a private network sends a request to the internet  
2. Router replaces the private IP with its public IP  
3. The request reaches the destination server  
4. Server sends response back to router’s public IP  
5. Router checks NAT table and forwards response to correct device  

---

## 🛠️ Types of NAT

### 1. Static NAT
- One-to-one mapping between private and public IP  
- Used for servers that need constant access  

---

### 2. Dynamic NAT
- Maps private IPs to a pool of public IPs  
- Assigned dynamically  

---

### 3. PAT (Port Address Translation)
- Also called NAT Overload  
- Many devices share a single public IP using port numbers  
- Most commonly used  

---

## 🧮 Example of NAT

### Private Network:
Device A → 192.168.1.2
Device B → 192.168.1.3

### Public IP:
Router → 203.0.113.1

### Translation:
| Private IP | Public IP |
|------------|----------|
| 192.168.1.2 | 203.0.113.1:1001 |
| 192.168.1.3 | 203.0.113.1:1002 |

---

## 🚀 Advantages
- Conserves public IP addresses  
- Enhances security (hides internal network)  
- Allows multiple devices to access the internet  
- Easy to implement  

---

## ⚠️ Disadvantages
- Can slow down network performance  
- Breaks end-to-end connectivity  
- Complicates some protocols (VoIP, gaming)  
- Requires additional configuration for port forwarding  

---

## 🔐 NAT and Security
NAT provides basic security by hiding internal IP addresses. However, it is not a replacement for firewalls.

---

## 📚 Conclusion
Network Address Translation (NAT) is a vital networking technique that enables efficient use of IP addresses and improves security. It plays a crucial role in modern networking by allowing multiple devices to communicate over the internet using a single public IP.

---

## 🔗 References
- RFC 2663 – NAT Terminology and Considerations  
- Cisco Networking Academy  
- Networking Fundamentals Books  
