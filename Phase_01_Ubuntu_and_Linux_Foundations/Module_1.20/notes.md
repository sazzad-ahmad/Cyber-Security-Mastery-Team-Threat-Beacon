# Module 1.20 — Linux Security Policies and PAM (Pluggable Authentication Modules)

## 🎯 Concepts Covered
- Pluggable Authentication Modules (PAM) Architecture
- PAM Service Configuration Directory (`/etc/pam.d/`)
- Management Group Types (`auth`, `account`, `password`, `session`)
- Control Flags (`required`, `requisite`, `sufficient`, `optional`)
- Enforcing Password Complexity & Lockout Policies

---

## 📌 Detailed Breakdown

### 1. PAM Architecture
- Dynamic layer abstracting authentication mechanisms away from system software/applications.
- Service definitions reside in `/etc/pam.d/` matching daemon names (e.g., `sshd`, `sudo`, `login`).

### 2. Management Modules
- **`auth`:** Validates user identity credentials.
- **`account`:** Verifies password expiration, temporal restrictions, and authorization scopes.
- **`password`:** Controls credential update pipelines and password complexity policies.
- **`session`:** Executes pre-login and post-logout environment configurations.

### 3. Security Engineering Applications
- Implementing `pam_faillock` or `pam_tally2` enforces automated account lockouts after consecutive failed authentication attempts, shutting down automated password brute-force vectors.
