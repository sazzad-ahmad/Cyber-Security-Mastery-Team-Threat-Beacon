# Module 0.3 — Operating System Fundamentals

## 🎯 Concepts Covered
- Operating System Architecture & Core Functions
- Kernel vs Shell
- Kernel Space vs User Space & System Calls
- Process Management, Threads, and System Services (Daemons)

---

## 📌 Detailed Breakdown

### 1. Kernel vs Shell
- **Kernel:** The core component of an OS managing hardware resources (CPU, RAM, Storage).
- **Shell:** Interface (CLI/GUI) translating user inputs into instructions for the kernel.

### 2. User Space vs Kernel Space
- **User Space:** Restricted memory area where user applications execute.
- **Kernel Space:** Unrestricted privileged memory area where the core kernel and device drivers run.
- **System Calls (Syscalls):** API bridging User Space applications with Kernel Space resources.

### 3. Processes & Daemons
- **Process:** An executing instance of a program residing in RAM.
- **Daemon/Service:** Background processes executing system-level tasks continuous execution.
