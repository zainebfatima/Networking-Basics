# 🌐 Router vs Switch – Networking Devices Report

## 📌 Introduction
Routers and switches are two fundamental networking devices used to connect devices and networks. Although both are essential for data communication, they serve different purposes and operate at different layers of the OSI model.

---

## 🎯 Objectives
- Understand the difference between routers and switches  
- Learn how they work and their roles in a network  
- Identify use cases for each device  
- Compare advantages and limitations  

---

## 📖 Key Concepts

### 1. Switch
A **switch** is a networking device that connects multiple devices within a **local area network (LAN)**.  
- Operates at **Layer 2 (Data Link Layer)**  
- Uses **MAC addresses** to forward data to the correct device  
- Can also operate at Layer 3 (some switches support routing)  

**Example:**PC1 → Switch → PC2

---

### 2. Router
A **router** connects **different networks** together, such as a LAN to the internet.  
- Operates at **Layer 3 (Network Layer)**  
- Uses **IP addresses** to forward packets between networks  
- Often includes NAT, DHCP, and firewall functions  

**Example:**LAN → Router → Internet

---

## ⚙️ Key Differences

| Feature               | Switch                        | Router                          |
|-----------------------|-------------------------------|---------------------------------|
| Function              | Connects devices in LAN       | Connects different networks     |
| OSI Layer             | Layer 2 (MAC)                | Layer 3 (IP)                    |
| Addressing            | MAC address                   | IP address                      |
| Data Forwarding       | Frames                        | Packets                         |
| Network Type          | LAN only                      | LAN, WAN                        |
| Devices Connected     | Multiple computers/devices    | Multiple networks                |
| Example Use           | Office LAN                     | Connecting home network to ISP  |

---

## 🛠️ How They Work Together
- Switches manage traffic **within a network**  
- Routers manage traffic **between networks**  
- Typical home/office setup:PCs → Switch → Router → Internet
- 
---

## 🚀 Advantages

### Switch
- Reduces network congestion  
- Efficient device-to-device communication  
- Supports VLANs for network segmentation  

### Router
- Connects multiple networks  
- Provides internet access  
- Can implement security and routing policies  

---

## ⚠️ Limitations

### Switch
- Cannot connect networks  
- Limited to local network communication  

### Router
- More expensive than switches  
- Slightly slower for local device-to-device communication  

---

## 📚 Conclusion
Switches and routers serve complementary roles in networking. Switches efficiently manage **internal LAN traffic**, while routers connect different networks and provide **internet access**. Understanding their differences helps in designing and managing networks effectively.

---

## 🔗 References
- Cisco Networking Basics  
- OSI Model Documentation  
- Networking textbooks and tutorials  
