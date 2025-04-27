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

| Model   | PCIe info | Read Speed | NVMe brand/model     | Notes |
|---------|-----------|------------|----------------------|-------|
| DS1823xs+ | 3.0 x8 slot (x4 link) | 2400 MB/s  |  | E10M20-T1 |
| DS1823xs+ | 3.0 x8 slot (x4 link) | 2400 MB/s  |  | M2D20 |
| DS1823xs+ | PCIe 3.0 x2 | 715 MB/s | WD Black SN850x 8TB | |
| DS1821+ | 3.0 x8 slot (x4 link) | 2350 MB/s  | WD Black SN770 500GB | E10M20-T1 |
| DS1821+ | 3.0 x8 slot (x4 link) | 2350 MB/s  | WD Black SN770 500GB | M2D20 |
| DS1821+ | PCIe 3.0 x2 | 1300 MB/s  | WD Black SN770 500GB |  |
| DS1621xs+ | PCIe 3.0 x2 | 2400 MB/s  | WD Black SN850 |  |
| DS1621xs+ | PCIe 3.0 x2 | 2400 MB/s  | Samsung SSD PM883 |  |
| DS1621+ | PCIe 3.0 x2 | 1300 MB/s  | 500GB | assumed to be the same as DS1821+ |
| DS1522+ | PCIe 3.0 x1 |  750 MB/s  | Samsung 980 Pro SSD 1TB |  |
| DS1520+ | PCIe 2.0 x1 |  400 MB/s  | Kingston KC3000 2048 GB | |
| DS1019+ | PCIe 2.0 x1 |  380 MB/s  | Intel SSDPEKKF512G8 512GB |  |
| DS1019+ | PCIe 2.0 x1 |  153 MB/s  | Inland Premium 1TB |  |
| DS923+  | PCIe 3.0 x1 |  750 MB/s  | | assumed to be the same as DS1522+ |
| DS920+  | PCIe 2.0 x1 |  390 MB/s  | Kingston NVME-SSD 1TB |  |
| DS918+  | PCIe 2.0 x1 |  400 MB/s  |  |  |
| DS723+  | PCIe 3.0 x1 |  730 MB/s  | | assumed to be the same as DS1522+ |
| DS720+  | PCIe 2.0 x1 |  400 MB/s  | Phison SPCC 500GB |  |
| DS720+  | PCIe 2.0 x1 |  390 MB/s  | WD Black SN770 500GB |  |
| DS720+  | PCIe 2.0 x1 |  390 MB/s  | Samsung Evo 970 2TB |  |
| DS423+  | PCIe 2.0 x1 |  740 MB/s  | Crucial P3 plus 2TB |  |
|  |  |  |  |  |
| RS3617RPxs | 3.0 x8 slot | 2055 MB/s | Samsung 970 EVO plus 1TB | [AliExpress cheap sinlge M2 adaptor card](https://www.aliexpress.com/item/1005002603686315.html) |
| RS1221+ | 3.0 x8 slot (x4 link) | 1465 MB/s | Samsung 980 1TB | E10M20-T1 |
