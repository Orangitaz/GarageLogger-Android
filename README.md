# Garage Log – Android

The [Garage Log](https://github.com/Orangitaz/GarageLogger) app packaged as an Android app. **It works on its own, with no server:** your data stays on the phone. If you also run Garage Log on a server (for example on TrueNAS), enter its address under **Settings & data > Server** and the phone syncs with it and with your other devices.

Without a server the phone can't send reminder alerts, check recalls, store documents or offer a calendar link, since those run on the server. Backups, CSV and service history go to the Android share sheet so you can save or send them.

## Get the APK
1. Open **Actions > Build Android APK > Run workflow**.
2. After about 5 minutes, open the run and download **garage-log-apk** under *Artifacts*, then unzip it.
3. Install the `.apk` on your phone (allow "install unknown apps" for the app you opened it from).

Every build bundles the latest version of the app from the main repository, so run the workflow again to update. The APK is signed with the key in `debug.keystore`, so a newer build installs over an older one and keeps your data.
