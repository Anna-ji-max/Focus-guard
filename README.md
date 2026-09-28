# FocusGuard

Phone-friendly Android project for FocusGuard.

## Build without a PC

This repository includes a GitHub Actions workflow. After uploading the project to a GitHub repository:

1. Open the repository on your phone.
2. Open **Actions**.
3. Select **Build FocusGuard APK**.
4. Tap **Run workflow** if it has not started automatically.
5. Wait for the workflow to finish.
6. Open the completed workflow run and download the **FocusGuard-debug-apk** artifact.
7. Extract the artifact and install `app-debug.apk` on Android.
8. Open FocusGuard and enable it under Android Accessibility / Installed apps.

The app uses an Accessibility Service to detect relevant Instagram UI and display local overlay reminders. Review and understand the requested accessibility access before enabling it.
