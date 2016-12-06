ffe-ath9k-blackout-workaround
==============================

This is a fork of ffho-ath9k-blackout-workaround ([Freifunk Hochstift](https://github.com/FreifunkHochstift/ffho-packages)).

In order to avoid further WiFi-Blackouts that *might* be caused by buggy ath9k,
this package tries to detect problems and restart the wifi.
If that doesn't work it tries to restart the nework and if even that fails, 
rebooting the node.

site.conf
---------

**ath9k_workaround.uptime_wait:**
- minimum uptime in minutes to perform actions 

**ath9k_workaround.blackout_wait:**
- minimum delay in minutes to detect a possible blackout as blackout

**ath9k_workaround.reset_wait:**
- minimum delay in minutes between wifi reset (command: wifi)

**ath9k_workaround.network_wait:**
- minimum delay in minutes between network reset (command: /etc/init.d/network restart)

**ath9k_workaround.reboot_wait:**
- minimum delay in minutes between reboot (command: reboot)

**ath9k_workaround.step_size**
- execute the cronjob each x minutes

### example
```lua
{
  ath9k_workaround = {
    reboot_wait = 240,
    network_wait = 120,
    uptime_wait = 20
    blackout_wait = 12,
    reset_wait = 10,
    step_size = 8,
  },
  ...
},
```
