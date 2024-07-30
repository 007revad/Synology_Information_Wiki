### Which Synology NAS models support WriteOnce and immutable snapshots?
https://kb.synology.com/en-global/DSM/tutorial/which_synology_nas_models_support_WriteOnce_and_secure_snapshots

<br>

Unofficially you can enable support for WriteOnce and immutable snapshots in older models (with DSM 7.2 or later)
```
sudo synosetkeyvalue /etc.defaults/synoinfo.conf support_worm yes
```
