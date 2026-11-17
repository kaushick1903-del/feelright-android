# FeelRight Android prototype

This folder wraps the FeelRight prototype (www/index.html) as an Android app with Capacitor.
Calls, huddles, hearts and login are simulated. Prototype OTP is 123456.

## Build the APK (on your computer)

You need: Node 20+, JDK 17+, Android Studio (it installs the Android SDK).

    npm install
    npx cap add android
    npx cap sync
    npm run apk

The APK appears at:

    android/app/build/outputs/apk/debug/app-debug.apk

Copy it to your phone, open it, and allow "Install unknown apps" when asked.

Or open it in Android Studio instead:

    npx cap open android      # then Build > Build APK(s)

## Change the app

Edit www/index.html, then run `npx cap sync` and build again.
Fonts load from Google Fonts, so the first launch needs internet. Without it the app uses system fonts.
