# Module 1.18 — Linux Firewall Management (UFW and iptables)

## 🎯 Concepts Covered
- Linux Kernel Netfilter Framework Architecture
- Low-Level Packet Filtering via `iptables` Tables and Chains
- High-Level Firewall Rule Management via Uncomplicated Firewall (`ufw`)
- Security Baselines: Default Deny Rules & Port Restrictions

---

## 📌 Detailed Breakdown

### 1. `iptables` Fundamentals
- **Chains:**
  - `INPUT`: Processes packets destined for the local system.
  - `OUTPUT`: Processes packets originating from the local system.
  - `FORWARD`: Processes packets routed through the local system.
- **Actions:** `ACCEPT`, `DROP` (silently discard), `REJECT` (discard with ICMP error notification).

### 2. UFW Operational Commands
- **`sudo ufw status verbose`:** Displays active rules and default policy stances.
- **`sudo ufw default deny incoming`:** Enforces zero-trust incoming packet policies.
- **`sudo ufw allow proto tcp from <IP> to any port 22`:** Granular IP/Port white-listing.
