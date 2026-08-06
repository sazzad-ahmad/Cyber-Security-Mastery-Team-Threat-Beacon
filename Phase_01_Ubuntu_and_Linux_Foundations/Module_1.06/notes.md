# Module 1.6 — Linux Permissions and Ownership

## 🎯 Concepts Covered
- File Ownership (User, Group, Others)
- Permission Triad (`r`, `w`, `x`) and Octal Notation (`4`, `2`, `1`)
- Changing Permissions (`chmod`) and Ownership (`chown`, `chgrp`)
- Special Permissions (SUID, SGID, Sticky Bit)

---

## 📌 Detailed Breakdown

### 1. Permission Mechanics
- **User (u):** Individual file creator or assigned user owner.
- **Group (g):** System group associated with the file.
- **Others (o):** All other authenticated system entities.

### 2. Octal Representation
- **Read (`r`):** 4
- **Write (`w`):** 2
- **Execute (`x`):** 1
- *Example:* `chmod 755` assigns `rwx` (Owner), `r-x` (Group), `r-x` (Others).

### 3. Special Permissions & Security Implications
- **SUID (`chmod u+s`):** Executes binary with owner privileges (critical attack vector for privilege escalation if misconfigured).
- **Sticky Bit (`chmod +t`):** Prevents non-owners from deleting files in world-writable directories like `/tmp`.
