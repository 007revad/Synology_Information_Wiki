### What type of fan speed modes are available on my Synology NAS?

https://kb.synology.com/en-ca/DSM/tutorial/What_type_of_fan_speed_modes_are_available_on_my_Synology_NAS

<br>

Some models run the fans at full or high speed when a network card is installed. This is configured by a setting in /etc.defaults/synoinfo.conf

For some reason Synology chose to run the fans at full speed for the RS2418RP+ and RS2418+
```
support_fan_adjust_by_ext_nic="full"

RS2418RP+
RS2418+
```

Yet for other models Synology set the fans to run at high speed (Cool Mode).
```
support_fan_adjust_by_ext_nic="high"

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

If you own an RS2418RP+ or RS2418+ and want to run the fans in cool mode with a network card installed:
```
sudo synosetkeyvalue /etc.defaults/synoinfo.conf support_fan_adjust_by_ext_nic high
sudo synosetkeyvalue /etc/synoinfo.conf support_fan_adjust_by_ext_nic high
```
So you don't have to do that after every DSM update you can set a scheduled task:
1. Go to **Control Panel** > **Task Scheduler** > click **Create** > and select **Triggered Task**.
2. Select **User-defined script**.
3. Enter a task name.
4. Select **root** as the user (The command needs to run as root).
5. Select **Boot-up** as the event that triggers the task.
6. Leave **Enable** ticked.
7. Click **Task Settings**.
8. Optionally you can tick **Send run details by email** and **Send run details only when the script terminates abnormally** then enter your email address.
9. In the box under **User-defined script** enter the following 2 lines. 
    ```
    /usr/syno/bin/synosetkeyvalue /etc.defaults/synoinfo.conf support_fan_adjust_by_ext_nic high
    /usr/syno/bin/synosetkeyvalue /etc/synoinfo.conf support_fan_adjust_by_ext_nic high
    ```
11. Click **OK** to save the settings.
