# Module 1.15 — Linux Security Basics and Hardening

## 🎯 Concepts Covered
- Linux Host Hardening Fundamentals & Principle of Least Privilege (PoLP)
- Host Firewall Configuration using Uncomplicated Firewall (`ufw`)
- SSH Server Hardening Mechanisms (`sshd_config`)
- Security Auditing & Baseline Compliance Inspections

---

## 📌 Detailed Breakdown

### 1. Uncomplicated Firewall (UFW)
- **Default Policy:** Deny all incoming traffic by default, allow outgoing traffic.
- **Rules Management:** Explicitly open necessary operational ports (`sudo ufw allow 22/tcp`).

### 2. SSH Hardening Guidelines (`/etc/ssh/sshd_config`)
- **`PermitRootLogin no`:** Prevents direct SSH privilege targeting on root.
- **`PasswordAuthentication no`:** Forces public-key cryptography to mitigate remote password brute-forcing attacks.
- **Non-Standard Port Allocation:** Changing default SSH Port `22` to mitigate automated scanner noise.

### 3. Baseline Audit Checklist
- Disabling unused services and closing unrequired open ports.
- Ensuring strict file permissions on critical assets (`/etc/shadow`, `/etc/sudoers`).
