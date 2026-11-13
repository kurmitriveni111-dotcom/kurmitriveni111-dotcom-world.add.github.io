FORMA X — ANDROID APK BUILD (PHONE-ONLY)
========================================

WHAT THIS IS
- A private Android wrapper around the supplied FORMA X HTML app.
- The build workflow creates a DEBUG APK for personal installation.
- This does not publish the app to Google Play or make it a public website.
- The app's 3D libraries may still need an internet connection because the HTML app loads some libraries from online CDNs.

IMPORTANT LIMITATIONS
- This is an unsigned debug APK, suitable for personal testing/installing. It is not a Play Store release.
- App projects/data are stored by the app's web storage on the device. Back up/export important projects.
- Android may ask you to allow installation from the browser or file manager you use to open the APK.
- The Android file picker and import support depend on the file types and Android version. Test your own files after installation.

BUILD IT USING ONLY YOUR ANDROID PHONE
1. Open GitHub in Chrome and sign in.
2. Create a NEW repository. Set it to PRIVATE. Name it: forma-x-android
3. Download this ZIP to your phone and extract it with Files / My Files.
4. Upload the CONTENTS of the extracted FORMA_X_Android_Build folder into the repository's main page. Make sure the .github/workflows/build-android.yml file is included. GitHub's mobile website may hide dot-folders; if so, use github.com in Chrome's Desktop site mode or the GitHub app/browser upload that shows hidden files.
5. Commit the files to the main branch.
6. In the repository, open Actions. Select “Build FORMA X Android APK”. If asked, enable GitHub Actions for the repository.
7. Open the latest running workflow and wait until it finishes with a green check mark.
8. Open that successful run, scroll to Artifacts, and tap “FORMA-X-Android-APK” to download the ZIP artifact.
9. Extract the downloaded artifact ZIP. Inside is app-debug.apk.
10. Tap app-debug.apk and follow Android's install prompts. If blocked, allow “Install unknown apps” for the browser or file manager you used, then retry.

IF THE BUILD FAILS
- Open the failed run, open the red failed step, and copy the error text.
- Do not share passwords, access tokens, or private keys. Send only the build error text for help.

PRIVACY
- Keep the GitHub repository PRIVATE.
- Do not add passwords, API keys, or personal project files to the repository.
- Anyone you explicitly give repository access to may be able to see its source files.
