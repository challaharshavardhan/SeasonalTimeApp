MUHURTA LOTUS - NATIVE ANDROID LAUNCHER ICON FIX

This is a complete Android Studio project, not just an HTML shortcut.
It uses the standard Android resource compiler (AAPT2) so Android can load the launcher icon.

BUILD
  1. Unzip this folder and open Muhurta-Lotus-AndroidStudio in Android Studio.
  2. Let Gradle sync (Android Studio may download necessary SDK/Gradle components).
  3. Use Build > Build Bundle(s) / APK(s) > Build APK(s).
  4. Find app-debug.apk in app/build/outputs/apk/debug/, copy to the phone, and install.

BEFORE INSTALLING
  This app's package ID is org.muhurta.lotus.gold, so it installs next to your old app.
  The older app and its saved preferences are not deleted.

WHAT IS CHANGED
  - Real Android launcher icon (standard PNGs in res/mipmap-*)
  - Real Android adaptive/round launcher icon (res/mipmap-anydpi-v26/)
  - Manifest declares android:icon and android:roundIcon
  - Original offline HTML is included byte-for-byte as assets/index.html
  - MainActivity uses a simple WebView with the original app's known settings

NOTE: This source project has been statically inspected but has not been built or
      tested on a physical device in this environment.

ALTERNATE BUILD VIA GITHUB ACTIONS
  Upload the contents of this project to a GitHub repository.
  Open Actions > Build Muhurta Lotus APK > Run workflow.
  Download the "Muhurta-Lotus-APK" artifact after the workflow succeeds.

The ZIP does NOT contain a compiled APK. An Android build is required.
