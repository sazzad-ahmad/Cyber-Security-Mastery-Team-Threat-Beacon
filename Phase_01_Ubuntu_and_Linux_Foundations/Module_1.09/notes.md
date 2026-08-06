# Module 1.9 — Linux Process Management

## 🎯 Concepts Covered
- Process Lifecycle & Execution States (Running, Sleeping, Zombie)
- Process Monitoring Utilities (`ps aux`, `top`, `htop`)
- Foreground vs Background Execution (`&`, `jobs`, `fg`, `bg`)
- Process Signals (`SIGTERM -15`, `SIGKILL -9`) and Termination (`kill`, `pkill`)

---

## 📌 Detailed Breakdown

### 1. Process Attributes
- **PID (Process ID):** Unique numerical identifier assigned to every running process.
- **PPID (Parent Process ID):** Identifier of the parent process that spawned the child execution.

### 2. Linux Signals & Termination
- **SIGTERM (Signal 15):** Graceful shutdown request allowing the application to clean up resources before exiting.
- **SIGKILL (Signal 9):** Immediate kernel-level process destruction; bypasses application cleanup handlers.

### 3. Security Relevance
- Detecting suspicious background processes running out of abnormal directories (e.g., unexpected processes executing from `/tmp` or `/dev/shm`).
