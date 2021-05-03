# VolumeControl

This app allows to bypass the high volume warning without root priviledges. </br>
It requires to reboot the device from time to time (or, alternatively, switch to another user and log in again).

This is a fork from [seamirage's original code](https://github.com/seamirage/VolumeControl) and the only difference is that I've built the [apk](app/build/outputs/apk/debug/app-debug.apk).


**How to use**
1. Download the [apk](app/build/outputs/apk/debug/app-debug.apk) 
2. Install it with adb:
  ```bash
  adb install -t app-debug.apk
  ```
3. Grant the permission 
  ```bash
   adb shell pm grant com.trueapps.volumecontrol android.permission.WRITE_SECURE_SETTINGS
  ```
4. Wait for a notification. It will be sent at the warning's approach.
