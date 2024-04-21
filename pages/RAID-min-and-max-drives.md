### From DSM 7.2.1 Storage Manager package

| RAID Type | Min Drives | Max Drives | Drive Redundancy | Support RAID Group |
|---------|---|--------|---|-----|
| SHR     | 1 | 65,536 | 1 | no  |
| SHR 2   | 4 | 65,536 | 2 | no  |
| RAID 1  | 2 | 4      | # disks -1 | no |
| RAID 5  | 3 | 65,536 | 1 | yes  |
| RAID 6  | 4 | 65,536 | 2 | yes  |
| RAID 10 | 4 | 65,536 | # disks /2 | no |
| Basic   | 1 | 1      | 0 | no  |
| JBOD    | 1 not RAID group | 65,536 | 0 | no |
| JBOD    | 2 with RAID Group | 65,536 | 0 | no |
| RAID 0  | 2 | 65,536 | 0 | no  |
| RAID F1 | 3 | 65,536 | 1 | yes |
