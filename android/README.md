# Expense Tracker Android App

This Android Studio project opens the deployed Expense Tracker web app (`https://expenselive.vercel.app/`), uses the custom Expense Tracker logo for the launcher icon and branded loading screen, and supports Android native camera receipt capture, offline error handling, and webview performance optimizations.

## Application Details
- **App Name**: Expense Tracker
- **Application ID / Package**: `com.expensetracker.app`
- **Target URL**: `https://expenselive.vercel.app/`
- **Version**: V2.6.0 (Version Code 18)

## Build an APK

### Signed Release APK
To build a production-signed release APK:
1. Keystore parameters in `local.properties`:
   ```properties
   RELEASE_STORE_FILE=expense-release.jks
   RELEASE_STORE_PASSWORD=ExpenseTracker@2026
   RELEASE_KEY_ALIAS=expensetracker
   RELEASE_KEY_PASSWORD=ExpenseTracker@2026
   ```
2. Run `./gradlew assembleRelease --no-daemon` from the `android` folder.
3. The signed APK is produced at `app/build/outputs/apk/release/Expense Tracker.V2.6.apk`.
