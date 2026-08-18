# Windows File System Forensics Lab: NTFS, FAT32 & FAT16

## Overview

This project documents a hands-on digital forensics laboratory designed to examine and compare **NTFS, FAT32, and FAT16 file systems** using Windows Disk Management and **Exterro FTK Imager**.

The lab was built from the ground up by creating three separate test disks, formatting each disk with a different file system, creating controlled evidence files, intentionally deleting selected files, and examining the resulting forensic artifacts.

The project demonstrates practical experience with Windows file systems, deleted-file analysis, Recycle Bin artifacts, hexadecimal data, file-system metadata, and unallocated space.

---

## Lab Objectives

The objectives of this project were to:

- Create three controlled test disks.
- Configure NTFS, FAT32, and FAT16 file systems.
- Create known text-based evidence.
- Intentionally delete selected evidence.
- Load physical disks into FTK Imager.
- Identify partitions and file-system structures.
- Examine active and deleted files.
- Investigate NTFS `$RECYCLE.BIN` artifacts.
- Compare deletion behavior across different file systems.
- Inspect raw hexadecimal data and unallocated space.

---

## Tools Used

| Tool | Purpose |
|---|---|
| Windows 11 | Laboratory operating environment |
| Windows Disk Management | Disk creation, partitioning, and formatting |
| Windows File Explorer | Evidence-file management |
| Notepad | Creation of controlled text evidence |
| Exterro FTK Imager | Forensic examination of physical disks |

---

## File Systems Examined

| Test Volume | File System |
|---|---|
| `NTFS_LAB` | NTFS |
| `FAT32_LAB` | FAT32 |
| `FAT_LAB` | FAT16 |

---

## Investigation Workflow

The laboratory followed this general forensic workflow:

1. Prepare three test disks.
2. Create and format the NTFS volume.
3. Create and format the FAT32 volume.
4. Create and format the FAT16 volume.
5. Create controlled text evidence.
6. Delete selected files.
7. Add the physical disks to FTK Imager.
8. Identify the three file-system structures.
9. Examine active files.
10. Locate deleted-file artifacts.
11. Investigate NTFS Recycle Bin artifacts.
12. Compare NTFS, FAT32, and FAT16 behavior.
13. Inspect hexadecimal data and unallocated space.
14. Document findings with forensic screenshots.

---

## Key Skills Demonstrated

- Digital forensics
- Windows file-system analysis
- NTFS analysis
- FAT32 analysis
- FAT16 analysis
- Deleted-file investigation
- Recycle Bin artifact analysis
- FTK Imager
- Hexadecimal inspection
- Unallocated-space analysis
- Evidence documentation
- Forensic methodology

---

## Project Documentation

The complete forensic workflow is documented across the following sections:

| Section | Documentation |
|---|---|
| 01 | [Evidence Creation](docs/01-evidence-creation.md) |
| 02 | [Controlled File Deletion](docs/02-controlled-file-deletion.md) |
| 03 | [FTK Imager Evidence Loading](docs/03-ftk-imager-evidence-loading.md) |
| 04 | [NTFS Forensic Analysis](docs/04-ntfs-forensic-analysis.md) |
| 05 | [FAT32 Forensic Analysis](docs/05-fat32-forensic-analysis.md) |
| 06 | [FAT16 Forensic Analysis](docs/06-fat16-forensic-analysis.md) |
| 07 | [File-System Forensic Comparison](docs/07-file-system-forensic-comparison.md) |

Each analysis section includes supporting screenshots collected during the FTK Imager examination.

---

## Key Findings

The investigation demonstrated that deleted data can remain forensically recoverable across NTFS, FAT32, and FAT16 file systems. FTK Imager provided visibility into active files, deleted-file artifacts, file-system metadata, Recycle Bin data, hexadecimal content, and unallocated space.

NTFS provided a more detailed file-system and metadata structure, while FAT32 and FAT16 demonstrated simpler structures while still retaining useful deleted-file evidence.

---

## Disclaimer

This project was performed in a controlled laboratory environment for educational and portfolio purposes. All files, disks, and deletion activity were intentionally created for forensic analysis.

---

## Author

**Anik Nohan**

Cybersecurity / SOC / Digital Forensics Portfolio
