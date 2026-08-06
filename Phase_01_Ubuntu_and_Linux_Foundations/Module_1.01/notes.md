# Module 1.1 — Ubuntu Installation Mastery

## 🎯 Concepts Covered
- Bare-Metal Installation vs Virtualization
- Disk Partitioning (`/`, `/home`, `swap`)
- Full Disk Encryption Mechanics (LUKS)
- Post-Installation Hardening Verification

---

## 📌 Detailed Breakdown

### 1. Partitioning Structure
- **`/` (Root Partition):** The top-level root directory containing system binaries and configurations.
- **`swap`:** Virtual memory fallback partition used when physical RAM capacity is exhausted.
- **`/home`:** Separate partition for user-specific data isolation.

### 2. Disk Encryption
- **LUKS (Linux Unified Key Setup):** Standard block-device encryption protocol providing confidentiality for data-at-rest against physical theft.
