# FAT32 Forensic Analysis

## Objective

The second file system examined in Exterro FTK Imager was the FAT32 test volume.

The purpose of this phase was to examine the FAT32 file-system structure and identify active files, deleted-file artifacts, Recycle Bin data, and unallocated space. The results were then compared with the artifacts observed during the NTFS examination.

---

## FAT32 Evidence Source

FTK Imager identified the FAT32 test disk as:

```text
\\.\PHYSICALDRIVE2
└── Partition 1 [201MB]
    └── FAT32_LAB [FAT32]
