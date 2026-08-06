# Module 1.2 — Linux Filesystem Hierarchy Standard (FHS)

## 🎯 Concepts Covered
- Linux Root Directory Structure (`/`)
- System Binaries (`/bin`, `/sbin`) vs System Configurations (`/etc`)
- Dynamic Data (`/var`) & System Logging (`/var/log`)
- Virtual Filesystems (`/proc`, `/sys`) & Temporary Storage (`/tmp`)

---

## 📌 Detailed Breakdown

### 1. Essential Directories
- **`/` (Root):** Top of the unified directory tree.
- **`/etc`:** Contains system-wide setup files and application configurations.
- **`/var/log`:** Primary repository for security logs, authentication attempts, and system audits.
- **`/proc`:** Virtual memory-backed filesystem exposing runtime kernel and active process states.
- **`/tmp`:** World-writable directory used for temporary files (frequent target for initial exploit staging).
