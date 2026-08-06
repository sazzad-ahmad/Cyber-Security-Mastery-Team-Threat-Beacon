# Module 1.13 — Linux Text Processing and Filtering

## 🎯 Concepts Covered
- Pattern Matching via `grep` & Regular Expressions (Regex)
- Column Processing & Stream Parsing via `awk`
- Inline Text Stream Editing via `sed`
- Stream Sorting (`sort`), Deduplication (`uniq`), and Truncation (`cut`)

---

## 📌 Detailed Breakdown

### 1. `grep` Utilities
- **`grep -i`:** Case-insensitive string filtering.
- **`grep -v`:** Inverted match returning non-matching lines.
- **`grep -E`:** Extended Regular Expressions (ERE) support for complex indicators of compromise (IoCs).

### 2. `awk` Mechanics
- Operates on record-based field variables (`$1`, `$2`, `$NF`).
- Useful for parsing standardized log formats (Apache/Nginx logs, `/etc/passwd`).

### 3. Pipeline Parsing (`sort | uniq -c`)
- Aggregating repeating records: Sorting stream inputs before passing to `uniq -c` enables frequency counting of IP addresses or brute-force attempt sources.
