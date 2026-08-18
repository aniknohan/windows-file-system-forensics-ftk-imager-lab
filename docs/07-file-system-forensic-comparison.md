# File-System Forensic Comparison

## Objective

The final phase of this project compared the forensic artifacts observed across the NTFS, FAT32, and FAT16 test volumes using Exterro FTK Imager.

The comparison focused on file-system structure, active files, deleted-file artifacts, Recycle Bin behavior, metadata, and unallocated space.

---

## NTFS vs FAT32 vs FAT16

| Feature | NTFS | FAT32 | FAT16 |
|---|---|---|---|
| File-system structure | More complex | Simpler | Simpler |
| Active file examination | Yes | Yes | Yes |
| Deleted-file artifacts | Identified | Identified | Identified |
| Recycle Bin artifacts | Present | Present | Present |
| File metadata | Detailed | Available | Available |
| Unallocated space | Identified | Identified | Identified |

---

## Key Observations

### NTFS

NTFS provided the most detailed file-system structure and metadata of the three examined file systems. FTK Imager allowed active files, deleted artifacts, Recycle Bin data, and unallocated space to be examined.

### FAT32

FAT32 used a simpler file-system structure while still retaining useful forensic evidence. Deleted files and their contents could remain recoverable after deletion.

### FAT16

FAT16 also demonstrated that file deletion does not necessarily remove file data immediately. Deleted-file entries, recoverable content, and unallocated space could still provide useful forensic evidence.

---

## Forensic Significance

The examination demonstrated that forensic evidence can persist across different Windows-compatible file systems after a user deletes a file.

Although NTFS, FAT32, and FAT16 organize data differently, FTK Imager was able to identify and examine active files, deleted artifacts, metadata, and unallocated space across the laboratory volumes.

This highlights an important principle of digital forensics: deleting a file does not necessarily mean that its underlying data has been immediately destroyed.

---

## Project Conclusion

This lab provided hands-on experience examining NTFS, FAT32, and FAT16 volumes with Exterro FTK Imager.

The investigation demonstrated practical skills in:

- Identifying file-system structures.
- Examining active files and metadata.
- Identifying deleted-file artifacts.
- Inspecting recoverable deleted content.
- Examining Recycle Bin artifacts.
- Reviewing unallocated space.
- Comparing forensic behavior across multiple file systems.

The project demonstrates a foundational Windows file-system forensic workflow and the use of FTK Imager for evidence examination and deleted-file analysis.
