# TCP & UDP - Beginner-Friendly Guide

Welcome! This repository will help beginners understand **TCP and UDP** in simple terms.

---

## 1️⃣ What is a Protocol?

A **protocol** is a set of **rules that computers follow to communicate** with each other over a network.

- Think of it as a **language** between devices.  
- TCP and UDP are **transport layer protocols** that define how data is sent and received.

---

## 2️⃣ What is TCP?

**TCP** stands for **Transmission Control Protocol**.

- It is **connection-oriented** → a connection is established before sending data.  
- Ensures **reliable delivery** of data packets.  
- Packets arrive **in the correct order**.  
- Lost packets are **retransmitted** automatically.

**Example:**  
Downloading a file from the internet uses TCP to make sure the file is complete and correct.

---

## 3️⃣ What is UDP?

**UDP** stands for **User Datagram Protocol**.

- It is **connectionless** → no connection is established before sending data.  
- **Faster** than TCP but **less reliable**.  
- Packets may **arrive out of order** or get lost.  
- Does **not retransmit lost packets**.

**Example:**  
Watching live video or playing an online game uses UDP because **speed is more important than perfect delivery**.

---

## 4️⃣ Why Do We Use TCP and UDP?

| Feature | TCP | UDP |
|---------|-----|-----|
| Speed | Slower | Faster |
| Reliability | Very reliable | Less reliable |
| Connection | Connection-oriented | Connectionless |
| Use Cases | Web browsing, Email, FTP | Streaming, Gaming, VoIP |

---

## 5️⃣ How TCP Works

TCP uses a **Three-Way Handshake** to establish a connection:

1. **SYN** → Client sends request to server.  
2. **SYN-ACK** → Server acknowledges request.  
3. **ACK** → Client confirms connection.  

After this, data transfer begins safely and reliably.

---

## 6️⃣ How UDP Works

- No handshake required.  
- Data packets are sent **immediately** without establishing a connection.  
- Faster but can lose packets.

---

## 7️⃣ Mini Quiz 🧠

**Q1.** What does TCP stand for?  
**Q2.** What does UDP stand for?  
**Q3.** Which protocol is connection-oriented?  
**Q4.** Which protocol is faster but less reliable?  
**Q5.** Which protocol guarantees packet delivery?  
**Q6.** Online gaming usually uses TCP or UDP?  
**Q7.** Which OSI layer do TCP and UDP belong to?  
**Q8.** What is the name of the 3-step process used by TCP to establish a connection?

---

  
