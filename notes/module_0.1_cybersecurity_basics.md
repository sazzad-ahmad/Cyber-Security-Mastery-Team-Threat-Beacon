# Module 0.1 — Cybersecurity Basics

## 1. Information Security vs Cyber Security
- **Information Security (InfoSec):** Protects all forms of data (both physical paper files and digital systems).
- **Cyber Security:** A subfield of InfoSec that specifically focuses on protecting digital assets, networks, and systems from online threats.

## 2. Ethical Hacking & Hacker Classifications
- **Ethical Hacking:** Authorized testing of an organization's systems to identify and remediate security vulnerabilities.
- **Hacker Types:**
  - **White Hat Hacker:** Ethical professionals authorized to perform security audits and penetration testing.
  - **Black Hat Hacker:** Malicious individuals who breach systems illegally for financial gain or damage.
  - **Gray Hat Hacker:** Unauthorized testers who find vulnerabilities without malicious intent, but act outside legal frameworks.

## 3. The CIA Triad
- **Confidentiality:** Ensures data is accessible only to authorized users.
  - *Mechanisms:* Encryption, Multi-Factor Authentication (2FA), Role-Based Access Control.
  - *Example:* Keeping banking PINs private.
- **Integrity:** Guarantees data has not been altered or tampered with by unauthorized parties.
  - *Mechanisms:* Hashing (SHA-256), Digital Signatures.
  - *Example:* Preventing unauthorized modification of financial balances.
- **Availability:** Ensures systems and services remain operational and accessible when needed.
  - *Mechanisms:* Redundancy, Backups, DDoS Protection.
  - *Example:* Maintaining uptime for emergency services.

## 4. Cyber Attack Lifecycle (Kill Chain Overview)
1. **Reconnaissance:** Gathering target information (IP addresses, open ports, technologies).
2. **Weaponization:** Coupling an exploit with a payload tailored to the vulnerability.
3. **Delivery:** Transmitting the payload to the target (e.g., via Phishing emails).
4. **Exploitation:** Executing code on the target system to leverage the vulnerability.
5. **Installation:** Establishing persistence (e.g., installing backdoors/malware).
6. **Command & Control (C2):** Establishing a remote management channel with the compromised host.
7. **Actions on Objectives:** Exfiltrating sensitive data, encrypting files, or causing disruption.

## 5. Legal & Ethical Boundaries
- **Authorization:** Testing any network or web application without explicit written consent (Statement of Work - SOW) is strictly illegal under cyber laws.
- **Responsible Disclosure:** Security researchers must notify system owners of discovered vulnerabilities privately and allow reasonable time for remediation before any public disclosure.
