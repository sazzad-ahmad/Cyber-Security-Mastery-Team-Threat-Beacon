# Module 1.10 — Linux System Services and systemd

## 🎯 Concepts Covered
- `systemd` Init System Architecture & Unit Files
- Managing Background Daemons via `systemctl`
- Service Lifecycle States (Active, Inactive, Failed)
- Service Persistence (`enable` vs `disable`) and Security Auditing

---

## 📌 Detailed Breakdown

### 1. `systemd` Framework
- **PID 1:** `systemd` acts as the first parent daemon initializing all operating system units.
- **Unit Files:** Configuration files residing in `/etc/systemd/system/` defining execution behavior, dependencies, and execution users for daemons.

### 2. Service Management (`systemctl`)
- **`systemctl status`:** Displays runtime health, logs, and process tree of a given service.
- **`systemctl enable/disable`:** Symlinks unit files to boot targets for auto-start execution control.

### 3. Security & Persistence Auditing
- Malicious persistence often utilizes unauthorized systemd service unit additions to ensure reboot survivability. Auditing enabled services via `systemctl list-unit-files` mitigates this risk.
