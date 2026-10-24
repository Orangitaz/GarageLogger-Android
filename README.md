# Garage Log – Android

<p>
<img src="https://raw.githubusercontent.com/Orangitaz/GarageLogger/main/screenshots/garage.png" width="31%" alt="My Garage">
<img src="https://raw.githubusercontent.com/Orangitaz/GarageLogger/main/screenshots/dashboard.png" width="31%" alt="Equipment dashboard">
<img src="https://raw.githubusercontent.com/Orangitaz/GarageLogger/main/screenshots/attention.png" width="31%" alt="Needs attention">
</p>

The [Garage Log](https://github.com/Orangitaz/GarageLogger) app packaged as an Android app. **It works on its own, with no server:** your data stays on the phone. If you also run Garage Log on a server (for example on TrueNAS), enter its address under **Settings & data > Server** and the phone syncs with it and with your other devices.

Without a server the phone can't send reminder alerts, check recalls, store documents or offer a calendar link, since those run on the server. Backups, CSV and service history go to the Android share sheet so you can save or send them.

## Get the APK
On your phone, open the **[latest release](../../releases/latest)** and tap **garage-log.apk**, or use the permanent link `https://github.com/Orangitaz/garagelogger-android/releases/latest/download/garage-log.apk`. Open the downloaded file and install it (allow "install unknown apps" for your browser when asked).

## Updating
A new release is built automatically (checked every 6 hours) whenever the main repository's `VERSION` changes. The app shows a green dot on the ⋯ button when a newer release exists; open **Settings & data > App updates** and tap the download link, then install over the old one. The APK is signed with the key in `debug.keystore`, so updates keep your data.

To build right away, open **Actions > Build Android APK > Run workflow** (tick *force* to rebuild a version that is already published).
Note: GitHub pauses scheduled runs after 60 days without repository activity; run the workflow once by hand to resume.
