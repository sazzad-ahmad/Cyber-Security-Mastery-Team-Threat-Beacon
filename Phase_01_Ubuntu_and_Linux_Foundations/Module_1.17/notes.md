# Module 1.17 — SSH and Remote Access Management

## 🎯 Concepts Covered
- SSH Architecture & Cryptographic Key Pairs (`Public` vs `Private`)
- Key-Based Authentication Workflow (`ssh-keygen`, `ssh-copy-id`)
- Secure File Transfer Utilities (`scp`, `rsync`, `sftp`)
- Hardening OpenSSH Server Configuration (`/etc/ssh/sshd_config`)

---

## 📌 Detailed Breakdown

### 1. Key Pair Cryptography
- **Private Key (`id_rsa`):** Remains strictly confidential on the client system (Permissions: `600`).
- **Public Key (`id_rsa.pub`):** Stored inside the remote host's `~/.ssh/authorized_keys` file (Permissions: `644`).

### 2. Operational Utilities
- **`ssh-keygen -t rsa -b 4096`:** Generates an RSA key-pair with 4096-bit length.
- **`scp localfile user@host:/path`:** Securely transfers files over SSH protocol layers.

### 3. Security Hardening Directives
- Restrict password authentication (`PasswordAuthentication no`).
- Restrict direct root interactive access (`PermitRootLogin no`).
- Bind SSH service to non-standard high ports to evade automated botnet scans.
