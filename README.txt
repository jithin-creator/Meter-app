# JJ METER SERVICE — Android APK project

This project builds a test/debug Android APK using GitHub Actions.

## Files
- `www/index.html` — app interface and meter record functions
- `www/jj-meter-logo.png` — JJ digital meter logo
- `capacitor.config.json` — Android app name and package ID
- `.github/workflows/build-apk.yml` — automatic APK build workflow

## Build on GitHub (Android phone steps)
1. Upload the contents of this folder into the root of your GitHub repository `jithin-creator/Bike-meter-manager`. Keep the `.github/workflows/build-apk.yml` path exactly as shown.
2. Commit the changes to the `main` branch.
3. Open the repository on GitHub and tap **Actions**.
4. Open **Build JJ METER SERVICE APK**. Wait for the workflow to finish with a green check mark.
5. Under the completed run, find **Artifacts** and download `JJ-METER-SERVICE-APK`.
6. Extract the downloaded ZIP and install `app-debug.apk`. Android may ask you to allow installation from that source.

## Important
- This creates a debug/test APK, not a Play Store release-signed APK.
- App records are saved in this app's local storage on the phone. Do regular JSON backups using the Backup button.
- QR libraries are loaded from the internet; QR generation/scanning needs internet access. Camera scanning requires camera permission.
- WhatsApp sharing opens WhatsApp's share/message screen; it does not send without your confirmation.
