# Module 1.11 — Linux Storage and File System Management

## 🎯 Concepts Covered
- Linux Block Devices (`/dev/sdX`, `/dev/nvmeXnY`)
- Common Linux Filesystems (`ext4`, `xfs`, `btrfs`)
- Partitioning (`fdisk`) & Formatting (`mkfs`) Mechanics
- Mounting Architecture & Mount Points (`mount`, `umount`, `/etc/fstab`)

---

## 📌 Detailed Breakdown

### 1. Storage Identifiers
- Block devices are referenced under the `/dev` pseudo-directory:
  - SATA/SCSI Drives: `/dev/sda`, `/dev/sdb`
  - NVMe Drives: `/dev/nvme0n1`

### 2. Mounting Mechanics
- **`mount`:** Binds a formatted filesystem partition to a directory path.
- **`umount`:** Safely unlinks a partition from its current mount point.
- **`/etc/fstab`:** Defines static persistent file system mounting configurations applied during system boot.

### 3. Forensic & Security Context
- Mounting evidence drives in Read-Only (`mount -o ro`) mode ensures zero evidence tampering during digital investigation workflows.
