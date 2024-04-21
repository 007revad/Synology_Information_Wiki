### Models that increase fan speed to high when PCIe network card is installed

In DSM 7.2 `/etc.defaults/synoinfo.conf` contains:

**Synology NAS with** `support_fan_adjust_by_ext_nic="full"`
   ```
RS2418RP+
RS2418+
   ```

**Synology NAS with** `support_fan_adjust_by_ext_nic="high"`
   ```
RS4021xs+
RS4017xs+
RS3621xs+
RS3621RPxs
RS3618xs
RS3617xs
RS3617xs+
RS3617RPxs
RS18017xs+
RS18016xs+
RS1619xs+
 
FS6400
FS3600
FS3410
FS3400
FS3017
FS2017

SA3610
SA3600
SA3410
SA3400D
SA3400
SA3200D

HD6500
   ```

**Possible Solution**

If you want the fans to run quieter try:

```
synosetkeyvalue /etc.defaults/synoinfo.conf support_fan_adjust_by_ext_nic "cool"
synosetkeyvalue /etc/synoinfo.conf support_fan_adjust_by_ext_nic "cool"
```
