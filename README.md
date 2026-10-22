# Loan Tracker (no server needed)

## On a laptop or phone
Double-click `index.html` to open it in your browser. No server, Python or internet connection is required.
Data is stored in the browser (localStorage). Always open the same file in the same browser.
Backup: use "Export backup" / "Import backup" at the bottom of the page.

Password: you create one on first launch and enter it every time you open the app.
It is a lock screen, not encryption. If you forget it, the only way back in is to reset (which deletes all data),
so export backups regularly.

## Menu, Settings and Contact
- Tap the menu button (top left) to open Home, Settings, Contact, a quick dark/light switch and Lock.
- Settings: Dark mode (System / Light / Dark, remembered), Change password, Export/Import backup.
- Contact: phone and email (tap to call or write).

## Android APK (Capacitor)
Requirements: Node.js (nodejs.org) and Android Studio (developer.android.com/studio)

1. Open a terminal in this folder and run:
   npm install
   npx cap add android
   npx cap sync android
2. Open the project in Android Studio:  npx cap open android
3. In Android Studio: Build > Build Bundle(s) / APK(s) > Build APK(s)
   The APK is at android/app/build/outputs/apk/debug/app-debug.apk. Install it on your phone.

When you change `index.html`, copy it to `www/index.html` and run `npx cap sync android` again.
To rename the app or package, edit `appId` and `appName` in capacitor.config.json.
