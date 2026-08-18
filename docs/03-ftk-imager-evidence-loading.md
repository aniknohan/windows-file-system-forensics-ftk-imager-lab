# FTK Imager Evidence Loading

## Objective

After creating and deleting the controlled evidence files, Exterro FTK Imager was used to examine the test disks from a forensic perspective.

The first step was to add the physical storage devices as evidence sources and verify that FTK Imager correctly identified their partitions and file systems.

---

## Tool

**Exterro FTK Imager 8.2.0.59 SP1**

FTK Imager provides an evidence-tree interface that allows an examiner to navigate physical disks, partitions, file systems, directories, files, and raw data.

---

## Adding the Physical Drive

FTK Imager was opened and the physical test disk was added as an evidence source.

After the evidence source was loaded, FTK Imager displayed the physical drive in the **Evidence Tree**.

The physical drive could then be expanded to reveal its partition and corresponding file system.

---

## NTFS Evidence Source

The first forensic test disk appeared in FTK Imager as:

```text
\\.\PHYSICALDRIVE1
└── Partition 1 [201MB]
    └── NTFS_LAB [NTFS]
