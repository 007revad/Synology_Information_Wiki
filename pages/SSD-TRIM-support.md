Enable SSD TRIM
- https://kb.synology.com/en-global/DSM/help/DSM/StorageManager/volume_ssd_trim?version=7
 
2.5" SATA SSD compatability - expand each one to check if TRIM is supported
- https://www.synology.com/en-global/compatibility?search_by=category&category=hdds_no_ssd_trim&filter_type=2.5%22%20SATA%20SSD&p=1&change_log_p=1

<br>

Models that don't support TRIM (checked in DSM 7.2.1)

```
DS116
DS119j
DS120j
DS216
DS216j
DS216play
DS218j
DS220j
DS223j
DS416
DS416j
DS416slim
RS217
RS816
```

#### M.2 drive TRIM support

DSM 7.1.1. has no SSD TRIM setting for M.2 storage pools

DSM 7.2 and later: 

| RAID Type | TRIM Supported |
|-----------|----------------|
| SHR |	yes |
| SHR-2 |	yes |
| RAID 1 |	yes |
| Basic |	yes |
| JBOD |	yes |
| RAID 0 |	**NO** |
| RAID 5 |	yes |
| RAID 6 |	yes |
| RAID 10 |  |
| RAID F1 |  |
