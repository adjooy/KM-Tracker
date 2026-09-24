# KM & Fuel Tracker — Android WebView

This project packages the supplied `index.html` panel as an Android WebView app.

## GitHub → APK

1. Create a new GitHub repository.
2. Upload all files/folders from this project to the repository.
3. Push to `main` (or `master`).
4. Open the **Actions** tab.
5. Run **Build APK** if it did not run automatically.
6. Open the completed workflow run.
7. Under **Artifacts**, download `KM-Fuel-Tracker-debug`.
8. Extract it and install `app-debug.apk` on Android.

## Important

The supplied HTML uses Firebase and external CDN libraries, so the Android app requests Internet access. The original HTML file is kept as `app/src/main/assets/index.html`.

The app also supports the HTML panel's JSON file picker used by Backup & Restore.

## Local build

Requires JDK 17, Android SDK, and Gradle 8.9:

```bash
gradle assembleDebug
```

APK output:

```text
app/build/outputs/apk/debug/app-debug.apk
```
