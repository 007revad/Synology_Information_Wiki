Officially no Synology NAS supports using M.2 drives in a PCIe card as a volume and they can only be used a cache.

Unofficially you can use https://github.com/007revad/Synology_M2_volume 


***

### E10M20-T1

https://www.synology.com/en-global/products/E10M20-T1#specs

```
NVMe SSD
  SA series: SA3600, SA3400, SA6400
  23 series: RS2423RP+, RS2423+
  22 series: RS822RP+, RS822+, DS3622xs+, DS2422+
  21 series: RS4021xs+, RS3621xs+, RS3621RPxs, RS2821RP+, RS2421RP+, RS2421+, RS1221RP+, RS1221+
  20 series: RS820RP+, RS820+
  19 series: DS2419+, DS2419+II, DS1819+
  18 series: RS3618xs, RS2818RP+, DS3018xs, DS1618+
  17 series: RS18017xs+, RS4017xs+, RS3617xs+, RS3617RPxs, DS3617xs, DS3617xsII
```

**Notes**
- DSM version requirement: 6.2.3-25426 or later version
- DSM version requirement for RS18017xs+, RS4017xs+, RS3618xs, RS3617xs+, RS3617RPxs, DS3617xs and DS3617xsII: 7.0.1 or later version


***

### M2D20

https://www.synology.com/en-global/products/M2D20#specs
```
NVMe SSD
  SA series: SA3600, SA3400, SA6400
  23 series: RS2423RP+, RS2423+
  22 series: RS822RP+, RS822+, DS3622xs+, DS2422+
  21 series: RS4021xs+, RS3621xs+, RS3621RPxs, RS2821RP+, RS2421RP+, RS2421+, RS1221RP+, RS1221+
  20 series: RS820RP+, RS820+
  19 series: DS2419+, DS2419+II, DS1819+
  18 series: RS3618xs, RS2818RP+, RS2418RP+, RS2418+, DS3018xs, DS1618+
  17 series: RS18017xs+, RS4017xs+, RS3617xs+, RS3617RPxs, DS3617xs, DS3617xsII
```


***

### M2D18

https://www.synology.com/en-global/products/M2D18#specs

```
NVMe & SATA SSD
  FS series: FS1018
  22 series: RS822RP+, RS822+
  21 series: RS1221RP+, RS1221+
  20 series: RS820RP+, RS820+
  19 series: DS2419+, DS2419+II, DS1819+
  18 series: RS2818RP+, RS2418RP+, RS2418+, DS3018xs, DS1618+
```

```
SATA SSD
  FS series: FS2017
  19 series: RS1219+
  18 series: RS3618xs, RS818RP+, RS818+
  17 series: RS18017xs+, RS4017xs+, RS3617xs+, RS3617RPxs, DS3617xs, DS3617xsII, DS1817+, DS1517+
```

**Notes**
- DSM version requirement: 6.2-23739-2 onward (or 6.1-15284-2 onward with DSM 6.1)
- Operating system requirement for RS1221RP+, RS1221+, RS822RP+, and RS822+: DSM 7.2-64551 or later.
- RS1221RP+, RS1221+, RS822RP+, and RS822+ support M.2 NVMe SSD with the M2D18 add-in card.
