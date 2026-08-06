# Module 1.16 — Linux Cron Jobs and Task Scheduling

## 🎯 Concepts Covered
- Cron Daemon (`crond`) & Crontab Architecture
- Crontab Time Field Syntax (`Minute Hour Day Month DayOfWeek`)
- Managing User Cron Jobs (`crontab -l`, `crontab -e`, `crontab -r`)
- System-Wide Cron Paths (`/etc/crontab`, `/etc/cron.d/`) and Persistence Auditing

---

## 📌 Detailed Breakdown

### 1. Crontab Time Syntax
* * * * *  <command_to_execute>
│ │ │ │ │
│ │ │ │ └──── Day of Week (0 - 6)
│ │ │ └────── Month (1 - 12)
│ │ └──────── Day of Month (1 - 31)
│ └────────── Hour (0 - 23)
└──────────── Minute (0 - 59)

### 2. Operational Utilities
- `crontab -l`: Enumerates scheduled entries for the authenticated user context.
- `crontab -e`: Opens standard text editor to add or modify periodic tasks.

### 3. Threat Hunting & Persistence Analysis
- Attackers frequently establish backdoors inside `/etc/cron.d/` or user crontabs to maintain non-interactive persistence across system reboots.
