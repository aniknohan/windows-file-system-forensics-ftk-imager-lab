# Controlled File Deletion Screenshots

This directory contains screenshots documenting the controlled file-deletion phase of the Windows file-system forensics laboratory.

Selected test files were intentionally deleted from the NTFS, FAT32, and FAT16 volumes to generate known deleted-file artifacts for later examination with Exterro FTK Imager.

The screenshots in this directory provide supporting evidence for:

[`docs/02-controlled-file-deletion.md`](../../../docs/02-controlled-file-deletion.md)

## Forensic Purpose

The controlled deletion process established a known baseline for examining how deleted files and related metadata are represented across different Windows file systems.

The resulting artifacts were later analyzed in FTK Imager to compare:

- NTFS deleted-file behavior
- FAT32 deleted-file behavior
- FAT16 deleted-file behavior
- Recycle Bin artifacts
- File-system metadata
- Recoverable file information
- Unallocated space

> All file creation and deletion activities were performed in a controlled laboratory environment using test data created specifically for forensic analysis.
