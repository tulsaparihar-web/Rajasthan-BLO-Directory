# Rajasthan BLO Directory — Build APK on GitHub

## Upload the Android project

1. Download the project ZIP from the ChatGPT conversation: `RajasthanBLODirectory_Project.zip`.
2. Open this repository: https://github.com/tulsaparihar-web/Rajasthan-BLO-Directory
3. Select **Add file → Upload files**.
4. Upload `RajasthanBLODirectory_Project.zip` at the repository root.
5. Commit the upload to `main`.

The **Build Rajasthan BLO Directory APK** workflow starts when the ZIP is added.

## Download the APK

1. Open the repository's **Actions** tab.
2. Select **Build Rajasthan BLO Directory APK**.
3. Open the latest successful run.
4. Download the `Rajasthan-BLO-Directory-APK` artifact.
5. Extract the artifact ZIP; it contains `app-debug.apk`.

This produces a debug APK for testing, not a signed production release. Before production, validate the contact-number field: it was mapped from the source workbook's `User Id` column and should be confirmed as valid dialable phone numbers. Also verify the app against the latest approved BLO data.

## Project ZIP

The ZIP is available in the original ChatGPT conversation as `RajasthanBLODirectory_Project.zip`. The GitHub connection used to prepare this repository can create text files, but cannot transfer that local ZIP binary automatically, so the one-time upload above is required.
