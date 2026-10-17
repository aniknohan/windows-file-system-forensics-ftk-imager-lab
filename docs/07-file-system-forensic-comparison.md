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

### Measured Results

| Observation | NTFS | FAT32 | FAT16 |
|---|---|---|---|
| Evidence source | `\\.\PHYSICALDRIVE1` | `\\.\PHYSICALDRIVE2` | `\\.\PHYSICALDRIVE3` |
| Volume label | `NTFS_LAB` | `FAT32_LAB` | `FAT_LAB` |
| Cluster size | 4,096 bytes | 2,048 bytes | 4,096 bytes |
| Key structures | `$MFT`, `$LogFile`, `$Bitmap`, `$MFTMirr` | `FAT1`, `FAT2`, `VBR`, reserved sectors | `FAT1`, `FAT2`, `VBR`, reserved sectors |
| Deleted entry in directory | Not listed in root | Shown with red X, `0xE5` marker | Shown with red X; name became `!ecret.txt` |
| Recycle Bin `$I`/`$R` pairs | 1 | 4 | 2 |
| Recovered `secret.txt` content | `$RY5NXTE.txt`: `Going be a CISO` | `$RPI0LC4.TXT`: `Going be a CISO` | `$RLXOD2W.TXT`: `Going be a CISO` |
| `evidence.txt` physical size (21-byte file) | 24 bytes | 2,048 bytes | 4,096 bytes |
| Timestamps | UTC | Local time | Local time |
| Unallocated regions | 3 | 2 | 3 |

The deleted file's content was recovered intact on **all three** file systems. The differences lie in the surrounding metadata: NTFS kept rich system structures and stored small-file data resident in the MFT; FAT32 and FAT16 kept deleted directory entries visible (marked with `0xE5`) and allocated whole clusters to tiny files, leaving file slack.

---

## Key Observations

### NTFS

NTFS provided the most detailed file-system structure and metadata of the three examined file systems. FTK Imager allowed active files, deleted artifacts, Recycle Bin data, and unallocated space to be examined.

### FAT32

FAT32 used a simpler file-system structure while still retaining useful forensic evidence. Deleted files and their contents could remain recoverable after deletion.

### FAT16

FAT16 also demonstrated that file deletion does not necessarily remove file data immediately. Deleted-file entries, recoverable content, and unallocated space could still provide useful forensic evidence.

### Timestamps

NTFS timestamps in FTK Imager appeared four hours later than Windows File Explorer's local time (UTC−4), consistent with NTFS storing UTC. FAT32 and FAT16 timestamps matched local time, and FTK Imager reported `UTC Timestamps: False` for both. Examiners must account for this when building timelines across file systems.

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
