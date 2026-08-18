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

Detailed walkthroughs and supporting forensic evidence will be organized in this repository as the investigation is documented.

---

## Disclaimer

This project was performed in a controlled laboratory environment for educational and portfolio purposes. All files, disks, and deletion activity were intentionally created for forensic analysis.

## Author

**Anik Nohan**

Cybersecurity / SOC / Digital Forensics Portfolio
