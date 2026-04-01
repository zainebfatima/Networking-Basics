# 🌐 Public vs Private IP Addresses – Networking Fundamentals Report

## 📌 Introduction
IP addresses are essential for devices to communicate over a network. They can be classified as **Public IP addresses** and **Private IP addresses**. Understanding the difference is crucial for networking, security, and internet connectivity.

---

## 🎯 Objectives
- Learn the difference between public and private IP addresses  
- Understand their usage and importance  
- Identify ranges for private IP addresses  
- Learn how devices communicate using public and private IPs  

---

## 📖 Key Concepts

### 1. Public IP Address
A **public IP address** is assigned to a device by an Internet Service Provider (ISP) and is **globally unique**.  
- Used to access the internet directly  
- Routable over the internet  
- Required for hosting websites, servers, or services  

**Example:**203.0.113.25

---

### 2. Private IP Address
A **private IP address** is used **within a local network** and is **not routable over the internet**.  
- Assigned by the network administrator or DHCP  
- Multiple networks can use the same private IP ranges  

**Private IP Ranges:**
- 10.0.0.0 – 10.255.255.255  
- 172.16.0.0 – 172.31.255.255  
- 192.168.0.0 – 192.168.255.255  

**Example:**192.168.1.10

---

## ⚙️ Key Differences

| Feature               | Public IP                  | Private IP                 |
|-----------------------|---------------------------|---------------------------|
| Visibility            | Accessible on the internet | Only accessible within LAN |
| Uniqueness            | Globally unique            | Unique only within LAN    |
| Assigned by           | ISP                        | Network administrator / DHCP |
| Usage                 | Internet communication     | Local network communication |
| Example               | 203.0.113.25               | 192.168.1.10              |

---

## 🛠️ How They Work Together
- Devices in a private network use private IPs  
- NAT (Network Address Translation) allows private IPs to communicate with the internet using a **single public IP**  
- This conserves public IP addresses and adds basic security  

**Example Setup:**Device A → 192.168.1.2 (private)
Router → 203.0.113.1 (public)

---

## 🚀 Advantages

### Public IP
- Globally unique and routable  
- Required for hosting services  
- Direct internet communication  

### Private IP
- Conserves public IP addresses  
- Enhances network security  
- Easy management of internal network  

---

## ⚠️ Limitations

### Public IP
- Limited availability  
- Vulnerable to attacks if not secured  

### Private IP
- Cannot access internet directly  
- Needs NAT to communicate outside the LAN  

---

## 📚 Conclusion
Public and private IP addresses work together to connect devices efficiently. **Private IPs** manage local networks securely, while **public IPs** allow communication over the internet. Understanding both types is essential for networking and internet setup.

---

## 🔗 References
- RFC 1918 – Address Allocation for Private Internets  
- Cisco Networking Fundamentals  
- Networking textbooks and online tutorials  
