# Module 1.7 — Linux User and Group Management

## 🎯 Concepts Covered
- User Account Types (Root, System, Regular)
- Essential System Files (`/etc/passwd`, `/etc/shadow`, `/etc/group`)
- User Creation & Modification (`useradd`, `adduser`, `usermod`, `userdel`)
- Group Mechanics & Privilege Control

---

## 📌 Detailed Breakdown

### 1. User Categorization & Identifiers
- **Root User (UID 0):** Absolute system controller with unconstrained system call privileges.
- **System Accounts (UID 1-999):** Non-interactive daemon service accounts.
- **Regular Users (UID 1000+):** Standard authenticated human or interactive session users.

### 2. Core Authentication Records
- **`/etc/passwd`:** World-readable plain text file mapping usernames, UIDs, GIDs, home directories, and login shells.
- **`/etc/shadow`:** Restrictive access file storing hashed user passwords and password expiration policies.
- **`/etc/group`:** Defines group structures and associated memberships.
