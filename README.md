# firmware_smartpro
Firmware release for TG5040 SmartPro

Firmware version: 1.0.3 - 20231222
=================================
1. Fix '?????' file name in non-English SD contents when using UMS mode.
2. SD card exFat/ntfs support in system, however only fat32 format can use for system update(uboot fat32).
3. Fn key editor. multi-seletion for cpu mode/LED/Silent/Global ABXYLR turbo fire/...
4. Fix Audio issues, add new battery features in Linux driver.
5. Theme refresh not complete issue
6. Press B key to move focus to top Tabs
7. Enable a lot of Linux drivers, like loop dev, more USB hid, add 1.8GHz cpufreq option.
   Add curl/wget in rootfs, add tftp/ftpd in busybox, keep libc/libstdc++ in 2.29 verison.
8. Search crashing issue.
9. Wifi records, wifi reconfig password, forget network.
10. Lock screen time setting.
11. Rumble motor level setting.
12. Fix game priview picture aspect.
13. Add function 'add to favorite' in search and recent page.
14. Add mute driver for Fn key.
15. Change Fn key to disable all previous items first. Active select items when exit editor.
16. Enable 'keymap-rotate 270' function.
         X
      Y     A
         B
      When enable 'rotate 270' and run games, the input map will switch to:
         Y
      B     X
         A
17. Fix netplay messages when using host-AP.
18. Fix SD readonly issue.
19. Change the default values when 'Factory Reset'.


Firmware version: 1.0.2 - 20231116
=================================
1. Joystick calibration zero center drift issue.
2. New Language setting, add UI language Korean.
3. Date/time, time zone setting.
4. CPU dynamic clock in MainUI and games.
5. USB Storage mode keep wakeup.
6. Game list preview thumbnail size changed.
7. Fix Main UI high CPU usage issue.
8. Fix key monitor daemon high CPU usage issue.

SD patch 20231115
=================================
1. RetroArch clear screen when exit.
2. PPSSPP L/R mapping issue.
3. RetroArch Shader setting save issue.
4. CPU dynamic clock in each Emus, named 'cpufreq.sh'.
   a. In most Emus, cpu clock will lock 1.008GHz in minimal.
   b. In 3D and big Emus, cpu clock will go performance governer.
   c. Use 'X' key in game list to pop up launching menu.

5. Change netplay timming to 60s per sync.




Firmware version: 1.0.0 - 20231105
=================================
First release.
