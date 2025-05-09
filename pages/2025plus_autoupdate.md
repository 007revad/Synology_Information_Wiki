DSM on 2025 and later Plus series (and probably also DSM 8 for all models) does not allow you to: 
- Set DSM to "Notify me and let me decide whether to install the new update".
- Set Package Center to not update packages automatically.

Synology have a provided a way, via SSH, to stop DSM or packages from updating automatically, but it stops both DSM and packages from auto updating.
https://kb.synology.com/en-global/DSM/tutorial/stop_system_package_auto_update

**Disable Package Center Auto Updates and DSM Auto Updates**
```
sudo /usr/libexec/syno-update-settings --set-autoupdatetype-notify
```

**Enable Package Center Auto Updates and DSM Auto Updates**
```
sudo /usr/libexec/syno-update-settings --unset-autoupdatetype-notify
```

<br>

## To prevent just DSM from auto updating:

**Disable DSM Auto Updates**
- Removes the schedule options in Control Panel > DSM Update > Settings
- We'll also disable those sneaky smart nano auto-updates
- Edit /usr/syno/etc/update.conf to <br>
```
{"autoupdate_type":"notify","smart_nano_enabled":false}
```

**Enable DSM Auto Updates**
- Restores the schedule options in Control Panel > DSM Update > Settings
- Edit /usr/syno/etc/update.conf to <br>
```
{"autoupdate_type":"hotfix-security","smart_nano_enabled":true}
```

<br>

## To prevent just packages from auto updating:

**Disable Package Center Auto Updates**
- Shows "Disable auto-update" option in Package Center > Setting > Auto-update
```
sudo synosetkeyvalue /etc/synoinfo.conf show_autoupdatetype_notify yes
```

**Enable Package Center Auto Updates**
- Removes "Disable auto-update" option in Package Center > Setting > Auto-update
```
sudo synosetkeyvalue /etc/synoinfo.conf show_autoupdatetype_notify no
```
