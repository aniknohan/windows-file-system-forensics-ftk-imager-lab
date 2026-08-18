# FAT16 Forensic Analysis

## Objective

The third file system examined in Exterro FTK Imager was the FAT16 test volume.

The purpose of this phase was to examine the FAT16 file-system structure and identify active files, deleted-file artifacts, Recycle Bin data, and unallocated space. This examination also provided a basis for comparing FAT16 with the previously analyzed NTFS and FAT32 volumes.

---

## FAT16 Evidence Source

FTK Imager identified the FAT16 test disk as:

```text
\\.\PHYSICALDRIVE3
└── Partition 1 [201MB]
    └── FAT_LAB [FAT16]
