# IPv4 Basics

## What is IPv4?

IPv4 (Internet Protocol version 4) is a 32-bit addressing system used to identify devices on a network.

Example:
192.168.1.1

---

## Structure

IPv4 address = 32 bits → divided into 4 octets.

Each octet ranges from 0–255.

---

## Network vs Host

* Network portion → identifies the network
* Host portion → identifies the device

Example:
192.168.1.10/24

Network: 192.168.1
Host: 10
# Lab 1: IP Calculation Practice

## Question

Find network, broadcast, and usable range for:

192.168.10.77/27

---

## Solution

Host bits = 32 − 27 = 5
Block size = 2^5 = 32

Ranges:
0–31
32–63
64–95 ← IP belongs here

Network: 192.168.10.64
Broadcast: 192.168.10.95
Usable: 192.168.10.65 – 192.168.10.94
