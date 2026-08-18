# FTK Imager Evidence Loading Screenshots

This directory contains screenshots documenting the process of loading the NTFS, FAT32, and FAT16 laboratory drives into Exterro FTK Imager as physical-drive evidence sources.

These screenshots support the forensic workflow documented in:

[`docs/03-ftk-imager-evidence-loading.md`](../../../docs/03-ftk-imager-evidence-loading.md)

## Evidence Loading

The screenshots in this directory demonstrate:

- Launching the FTK Imager evidence-loading workflow.
- Selecting `Physical Drive` as the evidence-source type.
- Selecting the appropriate laboratory physical drive.
- Loading the evidence source into the FTK Imager Evidence Tree.
- Identifying the corresponding partition and file system.

## Laboratory Evidence Sources

The following controlled volumes were examined:

- `NTFS_LAB` — NTFS
- `FAT32_LAB` — FAT32
- `FAT_LAB` — FAT16

These evidence sources were subsequently examined for active files, deleted-file artifacts, file-system metadata, hexadecimal data, and unallocated space.
