# Module 1.21 — SELinux and AppArmor Basics

## 🎯 Concepts Covered
- Discretionary Access Control (DAC) vs Mandatory Access Control (MAC)
- AppArmor Architecture & Profile Modes (`Enforce`, `Complain`, `Disabled`)
- SELinux Architecture & Operational Modes (`Enforcing`, `Permissive`, `Disabled`)
- Process Confinement & Zero-Day Exploit Mitigation

---

## 📌 Detailed Breakdown

### 1. DAC vs MAC
- **DAC:** standard Unix permissions (`rwx`) managed at the resource owner's discretion.
- **MAC:** Kernel-enforced security profiles strictly limiting system calls and file access paths regardless of standard user or root privileges.

### 2. AppArmor Mechanics (Ubuntu Default)
- Profiles are defined under `/etc/apparmor.d/`.
- **`aa-status`:** Audits running confined processes and active enforcement modes.
- **`aa-complain`:** Logs policy violations without blocking access (useful during application profile development).
- **`aa-enforce`:** Strictly blocks unauthorized file paths or socket creation attempts.

### 3. Exploit Mitigation
- Restricting application behavior ensures that even if a vulnerable web daemon (e.g., Apache/Nginx) is compromised, the attacker cannot pivot to sensitive system resources.
