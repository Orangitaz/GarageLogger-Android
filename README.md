# Garage Log – Android

A small Android wrapper for [Garage Log](https://github.com/Orangitaz/GarageLogger). On first launch it asks for your server address (e.g. `http://192.168.1.50:30080`), remembers it, and opens your Garage Log. Server updates show up automatically, so the APK rarely needs rebuilding.

## Get the APK
1. Open **Actions > Build Android APK > Run workflow**.
2. After about 4 minutes, open the run and download **garage-log-apk** under *Artifacts*, then unzip it.
3. Install the `.apk` on your phone (allow "install unknown apps" for the app you opened it from).

The APK is signed with the key in `debug.keystore`, so newer builds install over older ones. To change the server address later, clear the app's storage or reinstall.

Change `VERSION` to rename the APK (`garage-log-<version>.apk`).
