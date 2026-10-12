# Rajasthan BLO Directory

Bilingual Android directory for Booth Level Officers across Rajasthan.

## Build the APK

See [RAJASTHAN_BLO_APK_BUILD.md](RAJASTHAN_BLO_APK_BUILD.md) for instructions.

1. Upload `RajasthanBLODirectory_Project.zip` to the repository root.
2. Commit it to `main`; the GitHub Actions APK workflow will start automatically.
3. Open **Actions**, choose the successful **Build Rajasthan BLO Directory APK** run, and download the `Rajasthan-BLO-Directory-APK` artifact.

## Important data validation

The app's contact field was mapped from the original workbook's `User Id` column. Confirm that these values are valid dialable phone numbers before using the app in production. Validate the latest official BLO dataset and contact details before public release.
