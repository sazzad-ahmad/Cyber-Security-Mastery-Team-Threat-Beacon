# Module 1.14 — Linux System Logging and Auditing

## 🎯 Concepts Covered
- Linux Logging Infrastructure (`rsyslogd` vs `systemd-journald`)
- Critical Log Files (`/var/log/auth.log`, `/var/log/syslog`, `/var/log/kern.log`)
- Log Analysis via `journalctl` Utilities
- Kernel Level Auditing Mechanics (`auditd`)

---

## 📌 Detailed Breakdown

### 1. Critical Security Log Paths
- **`/var/log/auth.log`:** Tracks privilege escalation attempts, SSH logins, and authentication failures.
- **`/var/log/syslog`:** Central repository for non-security system events and application logs.
- **`/var/log/kern.log`:** Captures kernel-level warnings, hardware faults, and firewall drops.

### 2. `journalctl` Commands
- **`journalctl -f`:** Follow live log appends.
- **`journalctl -u <service>`:** Filter log streams dedicated to a target service daemon.
- **`journalctl -p err`:** Filter output based on log severity thresholds (Error, Critical, Alert, Emergency).

### 3. Security Auditing (`auditd`)
- Monitors file integrity (e.g., changes to `/etc/passwd` or `/etc/shadow`) and flags unauthorized system calls for digital forensics.
