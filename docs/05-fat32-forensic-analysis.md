# FAT32 Forensic Analysis

## Objective

The second file system examined in Exterro FTK Imager was the FAT32 test volume.

The purpose of this phase was to examine the FAT32 file-system structure, identify active and deleted file artifacts, inspect recoverable file content and metadata, and review unallocated space for residual data.

---

## FAT32 Evidence Source

FTK Imager identified the FAT32 test disk as:

```text
\\.\PHYSICALDRIVE2
└── Partition 1 [201MB]
    └── FAT32_LAB [FAT32]
