# frameXTV untuk Android TV

WebView wrapper ke https://framextv.xyz/

## Cara build APK
1. Install Android Studio (versi terbaru).
2. File > Open > pilih folder FrameXTV ini. Tunggu Gradle sync selesai.
3. Build > Build Bundle(s) / APK(s) > Build APK(s).
4. APK ada di app/build/outputs/apk/debug/app-debug.apk

## Install ke Android TV
- Lewat ADB: adb connect IP_TV:5555 lalu adb install app-debug.apk
- Atau copy APK ke flashdisk dan install pakai File Manager di TV.

## Ganti URL
Edit homeUrl dan allowedHost di MainActivity.kt

## Build tanpa Android Studio (GitHub Actions)
1. Upload semua isi folder ini ke repository GitHub (termasuk folder .github).
2. Buka tab Actions, jalankan workflow "Build APK" (atau tunggu otomatis setelah upload).
3. Setelah selesai, buka run-nya dan download artifact "frameXTV-apk".
