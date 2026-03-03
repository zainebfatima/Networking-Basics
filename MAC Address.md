# What is MAC Address?

**MAC = Media Access Control**  

It is a **unique physical address** assigned to your device’s network card (NIC).  

Think of it like:  
- **MAC** = your device’s fingerprint (permanent)  
- **IP** = your house address (can change)

---

## Example

If your laptop is connected to WiFi:
MAC Address: 00:1A:2B:3C:4D:5E

- First 3 pairs (00:1A:2B) → Manufacturer  
- Last 3 pairs (3C:4D:5E) → Device ID  

**Where is it stored?**  
Inside your device’s **Network Interface Card (NIC)**.  

---

## Why is MAC important?

- Helps devices in a **local network (LAN)** communicate  
- Can be used for **tracing devices** in limited scope  
- Cannot be used reliably for internet tracking
- # MAC Address Structure

## How many pairs and bits?

- MAC has **6 pairs** → 12 hexadecimal digits  
- Each digit = 4 bits → Total **48 bits**  
- Hexadecimal = 0–9, A–F

---

## First 3 pairs → Manufacturer

Example:
00:1A:2B

Check online at IEEE database → tells which company made the device

---

## Last 3 pairs → Device ID

- Unique to each device from manufacturer  
- Helps identify the device inside LAN  

**Note**: This is **not public info**, only manufacturer knows exact device

---

## Quick Diagram
00:1A:2B : 3C:4D:5E
|---------| Device ID
Manufacturer
# How MAC Helps in Tracing

## Scenario 1: Inside Organization

- Someone tries to hack LAN from inside office
- Switch logs show which MAC is on which port
- IT can trace device quickly because MAC is visible in LAN
- Example: Use `arp -a` to see IP ↔ MAC mapping

---

## Scenario 2: From Distance (Internet)

- Attacker comes from outside
- Only IP is visible in server logs
- MAC is **not visible** because MAC does not travel over internet
- You cannot track attacker using MAC in this case

---

## Limitations of MAC

- Only works in LAN  
- Can be **spoofed** (changed)  
- Cannot track over internet
- # What is ARP?

**ARP = Address Resolution Protocol**

- Translates **IP address → MAC address**  
- Example: Device wants to send data to 192.168.1.5  
- ARP asks: “Who has 192.168.1.5?”  
- Response: “MAC 00:1A:2B:3C:4D:5E”  

**Connection with MAC**: ARP allows devices to use MAC to send packets in LAN
# What is IP Lookup Database?

- Public database showing **IP ownership**  
- Shows: Country, ISP, Organization  
- Does NOT show personal info (only ISP can map IP → customer)

**Connection with MAC**:  
- Inside LAN → MAC identifies devices  
- Outside LAN → IP identifies devices, and you can look it up online
- # What is Timestamp?

- Timestamp = **exact time and date** when an event happened  
- Example in server log:
2026-03-03 21:42:15 IP: 39.45.12.100 Failed login
  
- Important because **IP changes over time**  
- Without timestamp, you cannot trace who used the IP at a specific moment
