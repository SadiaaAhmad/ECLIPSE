# ECLIPSE → downloadable phone app (Capacitor)

Your whole game is one folder: `index.html` + `assets/`. Capacitor wraps that exact folder into a
real installable **Android** (Play Store `.aab` / sideload `.apk`) and **iOS** app. No rewrite needed.

## One-time setup (on your computer)
1. Install **Node.js** (LTS) and, for Android, **Android Studio**. For iOS you need a Mac + Xcode.
2. Put the game in a `www` folder. Final layout:
   ```
   eclipse-app/
     www/
       index.html
       assets/...        (all your images + mp3s)
   ```
3. In a terminal, inside `eclipse-app/`:
   ```
   npm init -y
   npm install @capacitor/core @capacitor/cli @capacitor/android @capacitor/ios
   npx cap init "Eclipse" "com.yourname.eclipse" --web-dir=www
   npx cap add android
   npx cap add ios          # Mac only
   ```

## Each time you update the game
1. Copy the new `index.html` + `assets/` into `www/`.
2. `npx cap copy`
3. Android: `npx cap open android` → in Android Studio press **Run** (test) or **Build > Generate Signed Bundle/APK** (to ship).
   iOS: `npx cap open ios` → run/archive in Xcode.

## A few mobile niceties to add later (optional)
- **Lock to landscape** (this game is landscape): in `android/app/src/main/AndroidManifest.xml` add
  `android:screenOrientation="sensorLandscape"` to the `<activity>`. iOS: set Landscape-only in Xcode > Deployment Info.
- **Fullscreen / no status bar:** `npm install @capacitor/status-bar` and hide it on launch.
- **Keep screen awake during play:** `npm install @capacitor/keep-awake`.
- **App icon + splash:** `npm install @capacitor/assets`, drop a 1024×1024 icon + splash, run `npx capacitor-assets generate`.

## Publishing
- **Android:** create a Google Play Developer account ($25 one-time), upload the signed `.aab`.
- **iOS:** Apple Developer Program ($99/yr), upload via Xcode/Transporter to App Store Connect.

That's it — the game code never changes for packaging; it's purely a wrapper build step you do once you're happy.
