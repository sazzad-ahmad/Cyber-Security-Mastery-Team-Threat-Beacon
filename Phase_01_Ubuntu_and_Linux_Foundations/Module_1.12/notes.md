# Module 1.12 — Linux Networking Basics

## 🎯 Concepts Covered
- Network Interfaces & IP Addressing (`ip a`, `ip r`)
- Socket Statistics & Listening Ports (`ss -tulpn`)
- Connectivity Testing (`ping`, `traceroute`, `curl`)
- Domain Name Resolution (`dig`, `nslookup`)

---

## 📌 Detailed Breakdown

### 1. Interface & Route Inspection
- **`ip address` (`ip a`):** Enumerates system network interfaces, MAC addresses, and assigned IPv4/IPv6 addresses.
- **`ip route` (`ip r`):** Displays kernel routing table and default gateway paths.

### 2. Socket Statistics (`ss`)
- **`ss -tulpn`:** Crucial SOC tool for identifying listening ports and binding PIDs:
  - `-t`: TCP sockets
  - `-u`: UDP sockets
  - `-l`: Listening sockets
  - `-p`: Associated process ID/name
  - `-n`: Numeric port/address output

### 3. Security Analysis
- Unrecognized open ports running from unknown PIDs indicate potential rogue daemons or reverse shell connections.
