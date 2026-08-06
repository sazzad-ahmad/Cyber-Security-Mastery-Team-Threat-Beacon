# Module 1.23 — Linux System Monitoring and Performance Tuning

## 🎯 Concepts Covered
- Real-Time Resource Auditing via CLI Monitors (`top`, `htop`, `free`, `df`)
- Performance Bottleneck Identification (`vmstat`, `iostat`, `uptime`)
- Memory and Swap Space Utilization Mechanics
- Security Relevance: Detecting Cryptojacking, DoS Anomaly, and Rogue Processes

---

## 📌 Detailed Breakdown

### 1. Primary Monitoring Utilities
- **`free -m` / `free -h`:** Displays physical RAM usage, cached memory, and active swap partition spaces.
- **`df -h`:** Evaluates filesystem partition capacity usage in human-readable metrics.
- **`uptime`:** Provides total uptime along with Load Average metrics for 1-minute, 5-minute, and 15-minute intervals.

### 2. Advanced Performance Metrics
- **`vmstat 1 5`:** Reports virtual memory, CPU states, and process wait queues sampled every 1 second across 5 iterations.
- **`htop`:** Interactive, real-time process viewer allowing process tree inspection and immediate signal distribution (`SIGTERM`/`SIGKILL`).

### 3. Security Anomaly Detection
- Cryptomining malware or runaway rogue threads spike CPU usage to maximum thresholds. Monitoring tools allow rapid localization and termination of malicious process PIDs.
