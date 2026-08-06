# Module 1.19 — Linux Kernel and Module Management

## 🎯 Concepts Covered
- Monolithic Architecture vs Loadable Kernel Modules (LKM)
- Kernel Inspection Commands (`uname -r`, `lsmod`, `modinfo`)
- Dynamic Kernel Module Lifecycle (`modprobe`, `insmod`, `rmmod`)
- Security Relevance: Detecting Kernel-Level Rootkits and Malicious LKMs

---

## 📌 Detailed Breakdown

### 1. Loadable Kernel Modules (LKM)
- Code segments capable of dynamically extending kernel functionality at runtime without requiring a system reboot.
- Extension format: `.ko` (Kernel Object) files located under `/lib/modules/$(uname -r)/`.

### 2. Operational Utilities
- **`uname -r`:** Prints current operational kernel release.
- **`lsmod`:** Formats active modules currently running inside system RAM.
- **`modinfo`:** Inspects cryptographic signatures, author metadata, and parameters of specific kernel objects.
- **`modprobe`:** Smart module loader handling dependency resolutions automatically.

### 3. Forensic & Threat Analysis
- Threat actors leverage malicious LKMs (Kernel Rootkits) to intercept system calls, conceal files, network connections, and processes directly from user-land security utilities.
