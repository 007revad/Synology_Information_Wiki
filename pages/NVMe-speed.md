### NVMe read speeds per Synology model

If you want to check the read speed of your NVMe drive in your Synology NAS use:
```
sudo hdparm -tT --direct /dev/nvme0n1
```
or
```
sudo hdparm -tT --direct /dev/nvme1n1
```

To get your Synology's NVMe read speed added please [reply to this discussion](https://github.com/007revad/Synology_Information_Wiki/discussions/21).

<br>

| Model   | Read Speed | NVMe brand/model     | Notes |
|---------|------------|----------------------|-------|
| DS1821+ | 2350 MB/s  | WD Black SN770 500GB | E10M20-T1 |
| DS1821+ | 2350 MB/s  | WD Black SN770 500GB | M2D20 |
| DS1821+ | 1300 MB/s  | WD Black SN770 500GB |  |
| DS1621+ | 1300 MB/s  | 500GB | assumed to be the same as DS1821+ |
| DS1520+ |  390 MB/s  | 500GB | assumed to be the same as DS720+ |
| DS920+  |  390 MB/s  | 500GB | assumed to be the same as DS720+ |
| DS720+  |  390 MB/s  | WD Black SN770 500GB |  |

