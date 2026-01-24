In DSM 7.3.2 Synology increased the quiet and cool mode's fan speeds for the following models: 

- RS3618xs
- RS3621RPxs
- RS3621xs+
- RS4021xs+

DSM 7.3.2 for those modelss changed the PWM duty cycle for the Quiet and Cool fan settings in /usr/syno/etc.defaults/scemd.xml and /usr/syno/etc/scemd.xml.

In DSM 7.3.1 and earlier version they used to be:
```
Quiet Mode: pwm_duty_low="50" pwm_duty_high="220"
Cool Mode: pwm_duty_low="100" pwm_duty_high="220"
```

In DSM 7.3.2 they are now:
```
Quiet Mode: pwm_duty_low="100" pwm_duty_high="220"
Cool Mode: pwm_duty_low="120" pwm_duty_high="220"
```
