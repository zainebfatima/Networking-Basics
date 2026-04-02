# 📡 DHCP (Dynamic Host Configuration Protocol)

## 📌 Introduction
DHCP (Dynamic Host Configuration Protocol) is a network protocol used to automatically assign IP addresses and other network configuration settings to devices on a network. It eliminates the need for manual configuration.

---

## 🎯 Purpose of DHCP
- Automatically assigns IP addresses  
- Reduces configuration errors  
- Saves time for administrators  
- Efficiently manages IP allocation  

---

## ⚙️ How DHCP Works (DORA Process)

DHCP follows a 4-step process called DORA:

1. **Discover** – Client broadcasts request for DHCP server  
2. **Offer** – Server offers an IP address  
3. **Request** – Client requests the offered IP  
4. **Acknowledge (ACK)** – Server confirms and assigns IP  

---

## 📦 Information Provided by DHCP
- IP Address (e.g., 192.168.1.10)  
- Subnet Mask  
- Default Gateway  
- DNS Server  

---

## ⏱️ DHCP Lease Time
- IP is assigned for a limited time (lease)  
- Client renews lease before expiry  
- If renewal fails, a new IP is assigned  

---

## 🔁 Lease Renewal Process
- Happens automatically  
- Same IP is usually renewed  
- New IP is assigned only if needed  

---

## 🧩 DHCP Components

### 🔹 DHCP Server
- Assigns IP addresses  
- Usually a router in small networks  

### 🔹 DHCP Client
- Devices like computers, mobiles, printers  

### 🔹 DHCP Scope
- Range of IP addresses available  

---

## ⚖️ DHCP vs Static IP

| Feature | DHCP | Static IP |
|--------|------|----------|
| Configuration | Automatic | Manual |
| Stability | May change | Fixed |
| Usage | Home/School | Servers/Printers |

---

## 🚨 Common DHCP Issues

### 🔸 APIPA Address (169.254.x.x)
Occurs when DHCP server is not reachable  

### 🔸 IP Conflict
Two devices have same IP  

### 🔸 DHCP Server Down
No IP assigned to devices  

### 🔸 Limited IP Pool
New devices cannot connect  

---

## 🏫 Real-World Example
In a school network:
- Router acts as DHCP server  
- Devices get IP automatically  

Example:
- Student 1 → 192.168.1.2  
- Student 2 → 192.168.1.3  

---

## 💡 Best Practices
- Use DHCP Reservation for printers & servers  
- Set proper lease time  
- Monitor IP pool  
- Avoid multiple DHCP servers  

---

## ✅ Advantages
- Easy to manage  
- Saves time  
- Reduces errors  
- Scalable  

---

## ❌ Disadvantages
- Depends on DHCP server  
- IP may change  
- Security risks if misconfigured  

---

## 📚 Conclusion
DHCP is essential for modern networks. It automates IP assignment, reduces manual work, and ensures smooth connectivity in homes, schools, and organizations.
