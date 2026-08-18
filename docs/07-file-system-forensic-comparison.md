# File System Forensic Comparison: NTFS, FAT32, and FAT16

## Objective

This phase of the laboratory compares the forensic artifacts observed across the three controlled test file systems:

- NTFS
- FAT32
- FAT16

Each volume contained controlled test files and intentionally deleted artifacts. The volumes were examined using Exterro FTK Imager to determine how active files, deleted files, file-system metadata, Recycle Bin structures, and unallocated space appeared during forensic examination.

---

## Evidence Sources

Three physical test disks were examined.

| Physical Drive | Volume | File System | Approximate Partition Size |
|---|---|---|---:|
| `\\.\PHYSICALDRIVE1` | `NTFS_LAB` | NTFS | 201 MB |
| `\\.\PHYSICALDRIVE2` | `FAT32_LAB` | FAT32 | 201 MB |
| `\\.\PHYSICALDRIVE3` | `FAT_LAB` | FAT16 | 201 MB |

Using separate test volumes allowed similar file operations to be examined across different file-system structures.

---

## Controlled Evidence

The laboratory used known text files as controlled evidence.

Examples included:

```text
evidence.txt
notes.txt
secret.txt
