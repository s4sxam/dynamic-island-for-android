# Dynamic Island for Android

## Install on a phone

Open **Dynamic-Island.apk** on Android 10 or later. Tap **Install**, open **Dynamic Island** and tap **Start**. Follow the Android prompts and return to the app after each grant. The island starts automatically when setup finishes.

Android 11 and later may open the full **Display over other apps** list. Choose **Dynamic Island** there. If the notification-access switch is disabled on a sideloaded install, follow the in-app help to **App info → ⋮ → Allow restricted settings**, then return to notification access. Xiaomi devices may offer an additional **Background autostart** switch.

The pill appears briefly near the front camera when there is an event. Open the launcher icon to check status or stop the island. The app runs locally and its manifest requests no internet permission.

## Build the project

Open the extracted project in Android Studio with JDK 17, Android SDK platform 35 and build tools 34.0.0. From the project root on Windows, run `gradlew.bat :app:assembleDebug`. On macOS or Linux, run `sh gradlew :app:assembleDebug`. The debug APK is written to `app/build/outputs/apk/debug/`.

The project uses Gradle 8.9, Android Gradle Plugin 8.7.3, Kotlin 2.0.21 and Compose BOM 2024.12.01. The distributed APK uses a local release signing key. Android requires the same signing key for in-place updates.