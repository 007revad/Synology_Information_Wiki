## How to bring back the DSM update Notify option and Package Center Disable option

DSM 7.3 for all models (and DSM 7.2.2 for 25+ models):
- Removed the ability to prevent DSM auto updating.
- Removed the ability to prevent packages auto updating for 25+ and newer models.

But via SSH we can bring back the DSM updates notify option and the disable packages auto update option.

## DSM Auto Updates

Default DSM update settings:
<p align="left"><img src="pages/images/dsm_update_default.png"></p>

**To bring back the Notify option for DSM Updates:**

Via SSH:
```
sudo /usr/libexec/syno-update-settings --set-autoupdatetype-notify
```

Or in Task Scheduler create a "User defined script" scheduled task to run as root containing:
```
/usr/libexec/syno-update-settings --set-autoupdatetype-notify
```

Result:
<p align="left"><img src="pages/images/dsm_update_notify.png"></p>

**To restore it to default:**
```
sudo /usr/libexec/syno-update-settings --unset-autoupdatetype-notify
```

## Package Center Auto Updates

Default Package Center update settings:
<p align="left"><img src="pages/images/pkg_update_default.png"></p>

**To bring back the Disable Package Center Auto Updates option:**

Via SSH:
```
sudo synosetkeyvalue /etc/synoinfo.conf show_autoupdatetype_notify yes
```

Or in Task Scheduler create a "User defined script" scheduled task to run as root containing:
```
synosetkeyvalue /etc/synoinfo.conf show_autoupdatetype_notify yes
```

Result:
<p align="left"><img src="pages/images/pkg_update_disable.png"></p>

**To restore it to default:**
```
sudo synosetkeyvalue /etc/synoinfo.conf show_autoupdatetype_notify no
```
