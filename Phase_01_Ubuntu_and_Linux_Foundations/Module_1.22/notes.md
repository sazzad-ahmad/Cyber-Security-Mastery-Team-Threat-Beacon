# Module 1.22 — Linux Backup, Archiving, and Compression

## 🎯 Concepts Covered
- Tape Archive Mechanics (`tar`)
- Compression Algorithms (`gzip`, `bzip2`, `xz`)
- Incremental and Remote Data Synchronization (`rsync`)
- Forensic Data Preservation & Evidence Packaging

---

## 📌 Detailed Breakdown

### 1. `tar` Flag Specifications
- `-c`: Create a new archive.
- `-x`: Extract files from an archive.
- `-v`: Verbose output (list files processed).
- `-f`: Specify archive filename.
- `-z`: Filter archive through `gzip`.
- `-j`: Filter archive through `bzip2`.
- `-J`: Filter archive through `xz`.

### 2. Differential vs Incremental Backups (`rsync`)
- **`rsync -avz <source> <destination>`:**
  - `-a` (archive): Preserves permissions, symlinks, timestamps, and ownerships.
  - `-v` (verbose): Displays operation logs.
  - `-z` (compress): Compresses file data during transfer.

### 3. Digital Forensics Relevance
- Packaging compromised system artifacts using `tar -cJvf` ensures high-compression preservation while maintaining strict file permission metadata intact.
