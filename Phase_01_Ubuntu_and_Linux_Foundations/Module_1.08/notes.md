# Module 1.8 — Linux Package Management

## 🎯 Concepts Covered
- Package Architecture (`dpkg` vs `apt`)
- Debian Packages (`.deb`) & Repositories (`/etc/apt/sources.list`)
- System Updating (`update` vs `upgrade`) & Security Patching
- Package Maintenance (`autoremove`, `clean`)

---

## 📌 Detailed Breakdown

### 1. Package Managers Mechanics
- **`dpkg`:** Low-level Debian package manager operating directly on `.deb` archive binaries without automated dependency handling.
- **`apt`:** High-level package manager resolving software dependencies and downloading verified package releases via mirror repositories.

### 2. Repository Security
- Repository mirrors configured in `/etc/apt/sources.list` are cryptographically verified via GPG keys.
- Regular updates keep system libraries patched against known CVE vulnerabilities.
