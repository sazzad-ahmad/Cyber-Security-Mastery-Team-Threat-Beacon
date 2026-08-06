# Module 1.5 — Linux File and Directory Management

## 🎯 Concepts Covered
- File Creation (`touch`) & Reading Utilities (`cat`, `less`, `head`, `tail`)
- Directory Operations (`mkdir -p`, `rmdir`)
- Copying (`cp`), Moving/Renaming (`mv`), and Deleting (`rm -rf`)
- File Inspection Strategies for Log & Text Analysis

---

## 📌 Detailed Breakdown

### 1. File Inspection Utilities
- **`cat`:** Outputs whole file content to stdout (best for small text files).
- **`less`:** Paginated terminal interface suitable for viewing large system logs.
- **`head` / `tail`:** Inspects top or bottom N lines of a target file (`tail -f` streams live log appends).

### 2. File Manipulation Mechanics
- **`cp -r`:** Recursive copy flag required for directory hierarchies.
- **`mv`:** Relocates files or renames filenames within the same inode reference.
- **`rm -rf`:** Forces recursive removal without interactive prompts (high caution required).
