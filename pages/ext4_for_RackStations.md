### Enable creating ext4 volumes in DSM 7.2.1 on RackStations

In DSM 7.2.1 Synology disabled the ability to create ext4 volumes on RackStations.

You can enable it by running the following commands via SSH:
```
sudo synosetkeyvalue /etc/synoinfo.conf supportext4 yes
sudo synosetkeyvalue /etc.default/synoinfo.conf supportext4 yes
```
Then close and reopen storage manager. 

<br>

If you want to restore back to the default setting run the following commands via SSH:
```
sudo synosetkeyvalue /etc/synoinfo.conf supportext4 no_create
sudo synosetkeyvalue /etc.default/synoinfo.conf supportext4 no_create
```
Then close and reopen storage manager. 
