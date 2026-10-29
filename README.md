# Liquid Glass Home (Android)

A native Android launcher prototype inspired by the dark botanical / glass clock reference. Built for Vivo V2109 / Android 13, with app drawer and shortcuts to installed apps.

## Build on a phone (no computer)
### Option 1: AndroidIDE
1. Install AndroidIDE from its official project/release source.
2. Extract this ZIP in AndroidIDE or open the `LiquidGlassLauncher` folder.
3. Let Gradle sync. If asked, use JDK 17 and Android SDK platform 35.
4. Build > Assemble/Build APK.
5. Install the generated debug APK. Android may ask you to allow installs from that source.
6. Press Home and select **Liquid Glass Home**. If not prompted, open Settings and search for **Default apps > Home app**.

### Option 2: GitHub Actions (browser on your phone)
1. Create a GitHub repository and upload the contents of this folder (not the ZIP itself).
2. Add the workflow file `.github/workflows/build.yml` included in this project.
3. Open the repository's Actions tab and run the workflow.
4. Download the `LiquidGlass-debug-apk` artifact from the completed workflow, extract it, and install the APK.

## Important
- This is an iOS-inspired launcher, not a replacement operating system or an exact copy of Apple's OS.
- App opening uses installed Android app launch intents. A few favorites (YouTube, Chrome, Music, Photos) only work if those apps are installed.
- Native launcher icons and app drawer work, but the clock/weather/search cards are visual UI; the search card is a hint dialog, not a real web search.
- The project intentionally uses no third-party libraries.
