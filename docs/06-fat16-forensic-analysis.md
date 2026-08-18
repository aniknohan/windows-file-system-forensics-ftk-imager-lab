---

## FAT16 File-System Examination

FTK Imager identified the volume as `FAT_LAB [FAT16]`. The file system contained the root directory, FAT metadata, reserved sectors, and unallocated space.

![FAT16 file-system overview](../evidence/screenshots/06-fat16-forensic-analysis/01-fat16-file-system-overview.png)

---

## Root Directory Examination

The FAT16 root directory contained active files as well as deleted-file entries. Deleted entries were identified by the red X indicators displayed by FTK Imager.

![FAT16 root directory](../evidence/screenshots/06-fat16-forensic-analysis/02-fat16-root-directory-files.png)

---

## Deleted File Recovery

Deleted file artifacts remained accessible through the FAT16 file system and the Recycle Bin. FTK Imager allowed the contents of a deleted text file to be examined.

![FAT16 deleted file recovery](../evidence/screenshots/06-fat16-forensic-analysis/03-fat16-deleted-file-recovery.png)

---

## Active File Content

An active file named `evidence.txt` was examined. FTK Imager displayed the file content and associated metadata, demonstrating examination of an allocated file.

![FAT16 active file content](../evidence/screenshots/06-fat16-forensic-analysis/04-fat16-active-file-content.png)

---

## Unallocated Space

FTK Imager identified multiple regions of unallocated space within the FAT16 volume. These areas may contain residual data from previously deleted files.

![FAT16 unallocated space](../evidence/screenshots/06-fat16-forensic-analysis/05-fat16-unallocated-space.png)

---

## Key Findings

The FAT16 examination demonstrated:

- Identification of the FAT16 file-system structure.
- Examination of active and deleted files.
- Recovery and inspection of deleted-file content.
- Review of file metadata and contents.
- Identification of unallocated disk space.

These findings demonstrate how FTK Imager can be used to examine FAT16 file-system artifacts and recover evidence from deleted files.
