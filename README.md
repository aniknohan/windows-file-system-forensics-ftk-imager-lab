# Windows File System Forensics Investigation: NTFS, FAT32 & FAT16

## Overview

This project documents a hands-on digital forensics investigation designed to examine and compare **NTFS, FAT32, and FAT16 file systems** using Windows Disk Management and **Exterro FTK Imager**.

The forensic environment was built from the ground up by creating three separate test disks, formatting each disk with a different file system, creating controlled evidence files, intentionally deleting selected files, and examining the resulting forensic artifacts.

The project demonstrates practical experience with Windows file systems, deleted-file analysis, Recycle Bin artifacts, hexadecimal data, file-system metadata, and unallocated space.

---

## Investigation Objectives

The objectives of this project were to:

* Create three controlled forensic test disks.
* Configure NTFS, FAT32, and FAT16 file systems.
* Create known text-based evidence.
* Intentionally delete selected evidence files.
* Load physical disks into FTK Imager.
* Identify partitions and file-system structures.
* Examine active and deleted files.
* Investigate NTFS `$RECYCLE.BIN` artifacts.
* Compare deletion behavior across different file systems.
* Inspect raw hexadecimal data and unallocated space.
* Document forensic findings with supporting evidence.

---

## Tools Used

| Tool                    | Purpose                                                                                        |
| ----------------------- | ---------------------------------------------------------------------------------------------- |
| Windows 11              | Laboratory operating environment                                                               |
| Windows Disk Management | Disk creation, partitioning, and formatting                                                    |
| Windows File Explorer   | Controlled evidence-file management and deletion                                               |
| Notepad                 | Creation of controlled text evidence                                                           |
| Exterro FTK Imager      | Forensic examination of physical disks, file-system artifacts, hex data, and unallocated space |

---

## File Systems Examined

| Test Volume | File System |
| ----------- | ----------- |
| `NTFS_LAB`  | NTFS        |
| `FAT32_LAB` | FAT32       |
| `FAT_LAB`   | FAT16       |

---

## Investigation Workflow

The investigation followed a structured forensic workflow:

1. Prepare three dedicated test disks.
2. Create and format the NTFS volume.
3. Create and format the FAT32 volume.
4. Create and format the FAT16 volume.
5. Create controlled text-based evidence.
6. Intentionally delete selected files.
7. Add the physical disks to FTK Imager as evidence sources.
8. Identify the three file-system structures.
9. Examine active files and their contents.
10. Locate and analyze deleted-file artifacts.
11. Investigate NTFS Recycle Bin artifacts.
12. Compare NTFS, FAT32, and FAT16 deletion behavior.
13. Inspect hexadecimal data and unallocated space.
14. Document findings with supporting forensic screenshots.

---

## Key Skills Demonstrated

* Digital forensics
* Windows file-system analysis
* NTFS forensic analysis
* FAT32 forensic analysis
* FAT16 forensic analysis
* Deleted-file investigation
* NTFS Recycle Bin artifact analysis
* FTK Imager
* File-system metadata analysis
* Hexadecimal inspection
* Unallocated-space analysis
* Evidence interpretation and documentation
* Comparative forensic analysis
* Structured forensic methodology

---

## Project Documentation

The complete forensic workflow is documented across the following sections:

| Section | Documentation                                                                 |
| ------- | ----------------------------------------------------------------------------- |
| 01      | [Evidence Creation](docs/01-evidence-creation.md)                             |
| 02      | [Controlled File Deletion](docs/02-controlled-file-deletion.md)               |
| 03      | [FTK Imager Evidence Loading](docs/03-ftk-imager-evidence-loading.md)         |
| 04      | [NTFS Forensic Analysis](docs/04-ntfs-forensic-analysis.md)                   |
| 05      | [FAT32 Forensic Analysis](docs/05-fat32-forensic-analysis.md)                 |
| 06      | [FAT16 Forensic Analysis](docs/06-fat16-forensic-analysis.md)                 |
| 07      | [File-System Forensic Comparison](docs/07-file-system-forensic-comparison.md) |

Each analysis section includes supporting screenshots collected during the FTK Imager examination.

---

## Key Findings

The investigation demonstrated that deleting a file does not necessarily result in the immediate destruction of its underlying data. Depending on the file system and subsequent disk activity, deleted-file content and associated artifacts may remain available for forensic examination until the relevant storage areas are overwritten.

Key observations included:

* **NTFS** provided richer file-system metadata and forensic structures that offered additional context surrounding deleted files.
* NTFS `$RECYCLE.BIN` artifacts provided useful information for examining file-deletion activity.
* **FAT32** retained useful deleted-file artifacts despite using a simpler file-system structure than NTFS.
* **FAT16** also preserved evidence that could be identified and examined following controlled deletion.
* Hexadecimal inspection helped validate file content and residual evidence.
* Examination of unallocated space demonstrated how residual data may remain available for forensic analysis after file deletion.
* The forensic artifacts available after deletion varied depending on the underlying file system.

---

## Analyst Takeaways

This investigation demonstrated how **file-system architecture directly affects the forensic artifacts available during deleted-file analysis**.

NTFS provided richer metadata and Recycle Bin structures, while FAT32 and FAT16 used simpler file-system structures but still retained useful deleted-file evidence.

Comparing the same controlled deletion activity across all three file systems reinforced several important forensic principles:

* Deleted files may remain recoverable until their underlying data is overwritten.
* File-system metadata can provide investigative context beyond the contents of a deleted file.
* Available deletion artifacts vary depending on the underlying file system.
* Hex-level examination can help validate findings observed through higher-level forensic views.
* Unallocated space can be an important source of residual evidence.
* Understanding file-system behavior is important when interpreting deleted data during a forensic investigation.

Overall, this project strengthened my ability to examine Windows storage media, identify deleted-file artifacts, interpret file-system structures, validate evidence, and document forensic findings in a structured and repeatable manner.

---

## Disclaimer

This project was performed entirely within a **controlled laboratory environment** for educational and cybersecurity portfolio purposes.

All files, disks, evidence, and deletion activity were intentionally created for forensic analysis. No real-world systems or third-party data were involved.

---

## Author

**Anik Nohan**

Cybersecurity | SOC | Digital Forensics Portfolio

