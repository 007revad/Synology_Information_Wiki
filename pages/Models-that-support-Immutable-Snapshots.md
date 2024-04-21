Synology says Immutable Snapshots and WORM are only available on '20 series and newer models. 

https://kb.synology.com/en-global/DSM/tutorial/which_synology_nas_models_support_WriteOnce_and_secure_snapshots

| Series | Models |
|-----------|--|
| HD-series | HD6500 |
| FS-series | FS6400, FS3600, FS3410, FS3400, FS2500, FS2017, FS1018 |
| SA-series | SA6400, SA3610, SA3600, SA3410, SA3400, SA3400D, SA3200D |
| 24-series | DS224+ |
| 23-series | RS2423RP+, RS2423+, DS1823xs+, DS923+, DS723+, DS423+ |
| 22-series | RS822+, RS822RP+, RS422+, DS3622xs+, DS2422+, DS1522+ |
| 21-series | RS4021xs+, RS3621xs+, RS3621RPxs, RS2821RP+, RS2421+, RS2421RP+, RS1221+, RS1221RP+ <br> DS1821+, DS1621xs+, DS1621+ |
| 20-series | RS820+, RS820RP+ <br> DS1520+, DS920+, DS720+, DS620slim, DS420+, DS220+ |



<br>**NOTE:** I've had a report of the following causing issues on older models. https://github.com/007revad/Synology_HDD_db/issues/127 

We can enable them on other models that are using DSM 7.2 by running the following command:

```YAML
sudo synosetkeyvalue /etc.defaults/synoinfo.conf support_worm yes
```
Will that work on all models using DSM 7.2... I don't know. I've had reports that this does NOT work on older models.
