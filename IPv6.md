# IPv6 Basics

## What is IPv6?
IPv6 (Internet Protocol version 6) is the next-generation IP addressing system. It uses **128 bits**, compared to IPv4’s 32 bits, allowing for almost unlimited addresses.

Example:
2001:0db8:85a3:0000:0000:8a2e:0370:7334

---

## Structure
- IPv6 address has **8 blocks**, separated by colons
- Each block = 16 bits
- Total: 128 bits (8 × 16)

---

## Shortening IPv6
- Remove leading zeros in a block
- Replace consecutive blocks of zeros with `::` (once per address)

Example:
2001:0db8:0000:0000:0000:0000:0000:0001 → 2001:db8::1

---

## Network vs Host
- IPv6 usually splits 128 bits as:
  - First 64 bits → Network
  - Last 64 bits → Host

Example:
2001:db8:abcd:0012::1/64  
- Network: 2001:db8:abcd:0012::  
- Host: 1

---

## IPv6 Advantages
- Huge address space  
- Built-in IPsec security  
- No NAT required (direct addressing)  
- Easier autoconfiguration  

## IPv6 Risks
- Direct device exposure if firewall misconfigured  
- New attack surfaces for hackers
# IPv6 Subnetting Lab

## Question
Given IPv6 address: 2001:db8:abcd:0012::1/64  
Find:

- Network address  
- Host range (first and last host)  
- Broadcast equivalent (note: IPv6 does not use traditional broadcast)

---

## Solution

### Step 1: Identify Network and Host
Prefix = /64 → First 64 bits = network  
Last 64 bits = host portion

### Step 2: Network Address
2001:db8:abcd:0012::  
(all host bits are zeros)

### Step 3: Host Range
First host: 2001:db8:abcd:0012::1  
Last host: 2001:db8:abcd:0012:ffff:ffff:ffff:ffff

### Step 4: Broadcast
IPv6 does not have broadcast; it uses **multicast** instead.
