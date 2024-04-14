# firmware_smartpro
Firmware release for TG5040 SmartPro

Firmware version: 1.0.4 hotfix - 20240413
=================================
1. Fix manually time setting issue. (App hang or suspend failed)
2. Add libFlac for MAME RetroArch core.
3. Fix random key hang issue when wakeup.
4. Make Wi-Fi static mac address.

Firmware version: 1.0.4 - 20240401
=================================
1. Enable bluetooth function, support a2dp audio and BLE hid. Enable bluetooth audio to all alsa applications.
2. Add Vulkan Linux driver, update GLES/Vulkan library blobs from 1.11 to 1.19.
   SDL2 enabled vulkan support.
   More updates please check SD base package.
      Fix tmntsr graphic corruption
      Fix PPSSPP graphic corruption
      Enable RetroArch vulkan support.

3. Update rootfs libc to version 2.33.
4. Add Media Player with hardware decoding base on TinaPlayer.
   Video:
      H265 MP/L5.2 4k@30fps 100Mbps
      H.264 BP/MP/HP Level5.1 1080p@60fps 60Mbps
      AVS/AVS+ 1080p@60fps 30Mbps
      VP8 N/A 1080p@60fps 40Mbps
      MPEG1 MP/HL 1080p@60fps 100Mbps
      MPEG2 MP/HL 1080p@60fps 100Mbps
      MPEG4 SP/ASP L5 1080p@60fps 100Mbps
      XVID N/A 1080p@60fps 100Mbps
      H.263 BP 1080p@60fps 100Mbps
      Sorenson Spark N/A 1080p@60fps 100Mbps
      WMV9/VC-1 SP/MP/AP 1080p@30fps 100Mbps
      MJPEG N/A 1080p@60fps 60Mbps

   Audio:
      aac、mp3、ape、ogg、flac、wav、opus、alac、amr

   Not support:
      Dolby, AC3.

5. Add moonlight streaming for NVidia or Sunshine (select + start quit streaming)
    Notice!  Please turn bluetooth off when streaming. Bluetooth function will have performance impact on WiFi.

6. Add display enhance color setting.
7. Battery updates
      Modify charging current from 1500mA to 1950mA. 
      Add low battery warning (Joystick LEDs).
      Add low battery wakeup and auto shutdown.
      Power key long pressing 1.5s to force quit app, long pressing 6s to normally shutdown.

8. Wi-Fi driver updated to reduce suspend cancelling (auto screen on when power key suspend).
9. Add Language 'traditional-Chinese/German/French/Italian/Russian'.
10. Fix search result issue when returning from game.
11. Fix 'Refresh roms' issue in 'Best' tab.
12. Fix config.json issue when using png as value of key 'extlist'.
13. Turn off Wi-Fi when suspend, fix auto wakeup when pressing power key (after 15 seconds).
14. Add built-in SD FAT32 formatter.
15. Add new tab named 'Ports' for standalone games in 'Ports' folder in SD root path.


Firmware version: 1.0.3 - 20240320 hotfix
=================================
1. Fix some LCD timing issue.


Firmware version: 1.0.3 - 20240105 hotfix
=================================
1. Fix audio issue: volume is not actually zero when adjusting to zero.


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
