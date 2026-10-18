# Garage Log (Android)
A WebView wrapper around the Garage Log web app. The app lives in app/src/main/assets/index.html.
Data is cached on the phone and syncs to your TrueNAS Garage Log server.
On first launch the settings screen opens: enter the server address (for example http://192.168.1.50:30500) and tap Save & sync.
You can change it later under the three dots menu. Without a reachable server the app keeps working from the phone's copy.
Phone and NAS must be on the same network (or connected by VPN). Use Backup in the same menu before uninstalling.

## Build option A: GitHub (no installs)
1. Create a new private GitHub repo and upload everything in this folder (keep .github/workflows).
2. Open the Actions tab > "Build APK" > Run workflow (it also runs on every push).
3. When it finishes, download the "garage-log-apk" artifact, unzip it, and copy app-debug.apk to your phone.

## Build option B: Android Studio
Open this folder, wait for the Gradle sync, then Build > Build APK(s). Output: app/build/outputs/apk/debug/app-debug.apk

## Install
Open the APK on the phone and allow "install unknown apps" for the app you opened it from.
To update the web app later, replace app/src/main/assets/index.html and rebuild.
