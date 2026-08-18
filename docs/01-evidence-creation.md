# Evidence File Creation

## Objective

The first phase of this lab involved creating controlled text files that would later be examined using Exterro FTK Imager.

The purpose was to create known evidence, perform controlled file deletion, and then compare how the resulting artifacts appeared across NTFS, FAT32, and FAT16 file systems.

---

## Test File Systems

Three separate test volumes were used during the lab:

| Volume | File System |
|---|---|
| `NTFS_LAB` | NTFS |
| `FAT32_LAB` | FAT32 |
| `FAT_LAB` | FAT16 |

Using separate volumes allowed the same general evidence scenario to be examined across different Windows file systems.

---

## Evidence Files

The lab used three small text files:

- `evidence.txt`
- `notes.txt`
- `secret.txt`

The files contained simple, recognizable text so their contents could later be identified during forensic examination.

---

## NTFS Test Files

The files were created on the `NTFS_LAB` volume.

The NTFS test environment contained:

```text
evidence.txt
notes.txt
secret.txt
