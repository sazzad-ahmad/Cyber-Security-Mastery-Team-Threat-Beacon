# Module 1.3 — Linux Boot Process

## 🎯 Concepts Covered
- The 6 Stages of Linux Booting (BIOS/UEFI to systemd)
- GRUB Bootloader Configuration
- Kernel Initialization & Initramfs Mechanics
- Initialization System (`systemd` with PID 1)

---

## 📌 Detailed Breakdown

### 1. Boot Stages
1. **BIOS/UEFI:** Hardware initialization and boot device selection.
2. **POST:** Self-test ensuring basic hardware validity.
3. **GRUB:** Bootloader facilitating kernel selection and loading into RAM.
4. **Kernel:** Mounts root filesystem and sets up system drivers.
5. **Initramfs:** Temporary RAM-based root environment used during boot setup.
6. **systemd (PID 1):** Primary parent process initializing all background system services.

### 2. Security Analysis
- Inspecting GRUB configurations for unauthorized boot parameter modifications.
- Analyzing boot times and services via `systemd-analyze` to detect persistence mechanisms.
