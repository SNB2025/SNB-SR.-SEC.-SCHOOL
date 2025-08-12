# SNB SR.SEC.SCHOOL — Android App
A complete digital solution for managing and enhancing the school experience for students, parents, and staff.
A lightweight, secure Android WebView app for accessing the SNB Senior Secondary School portal.

- **Package ID**: `com.mrcpkm.snbsrsecschool`
- **Update source**: GitHub Releases of this repo

### Minimum system requirements
- **OS**: Android 10 (API 29) or higher
- **CPU/RAM**: Any device capable of running Android 10; 2 GB RAM recommended
- **Storage**: ~10–30 MB free (APK size varies by build type)
- **Network**: Internet connection for live content; cached content can show offline

### Download and installation
- Download the latest APK from Releases.
- On your phone, open the APK and follow the installation prompts.
- If blocked, enable “Install unknown apps” for your browser or file manager.

### Key features
- **Pull-to-refresh**
- **Offline screen with Retry** when no internet is available
- **Caching**: Uses cached content when offline; fetches fresh data when online
- **Auto-refresh on resume** to keep content up-to-date
- **Exit confirmation** on back press
- **Encrypted storage** of minimal local data
- **In-app update check** (GitHub Releases)
- **Update prompt with no-decline**: shows current and latest versions; only “Update” button
- **External URL blocking**: navigation restricted to the school domain
- **Screenshot/recording prevention** for security
- **Small APK size** with code shrinking and resource shrinking enabled

### Permissions used
- `INTERNET`: Load site content
- `ACCESS_NETWORK_STATE`: Detect connectivity for offline handling

### Privacy and security
- No analytics, no background trackers
- Uses Android EncryptedSharedPreferences (AES-256) for small local values
- Disables screenshots and screen recording at the window level
- Cleartext traffic is disabled

### In-app updates (how it works)
- On app launch, the app silently checks the latest release via GitHub API.
- Compares your installed `versionName` to the release `tag_name` (e.g., v1.0.0).
- If newer is available, a non-cancelable dialog appears:
  - Shows “Current version” and “Latest version”
  - Only “Update” button, which opens the APK asset or the release page.

Reference release link: [v1.0.0](https://github.com/SNB2025/SNB-SR.-SEC.-SCHOOL/releases/tag/v1.0.0)

### Offline and caching behavior
- When online: loads fresh content and updates cache.
- When offline: shows a friendly offline screen with a Retry button; attempts to use cache with WebView’s cache mode.

### Known limitations
- The app blocks navigation outside the main domain for safety. Links to other domains won’t open inside the app.
- File upload/download inside WebView is not customized; default WebView behavior applies.

### Changelog template
- v1.0.0
  - Initial public release
  - WebView, pull-to-refresh, offline screen + retry
  - Caching + auto-refresh on resume
  - Encrypted storage, forced-update dialog, screenshot prevention
  - External link blocking, minimized APK with shrinker

### Troubleshooting
- Stuck on offline screen:
  - Check your internet, pull-to-refresh, or tap Retry.
  - Ensure the app has network permissions; try toggling airplane mode.
- Update dialog keeps appearing:
  - Install the latest APK from Releases.



SCREENSHOTS:

![Image Alt](https://github.com/SNB2025/SNB-SR.-SEC.-SCHOOL/blob/299c6ee44d7ececbf6361626d2e67edfaa3101cd/photo_11_2025-08-09_11-18-05.jpg)

![Image Alt](https://github.com/SNB2025/SNB-SR.-SEC.-SCHOOL/blob/58bbfed6a3732c16146782e8441d2703934c1215/photo_13_2025-08-09_11-18-05.jpg)

![Image Alt](https://github.com/SNB2025/SNB-SR.-SEC.-SCHOOL/blob/58bbfed6a3732c16146782e8441d2703934c1215/photo_1_2025-08-09_11-18-05.jpg)

![Image Alt](https://github.com/SNB2025/SNB-SR.-SEC.-SCHOOL/blob/58bbfed6a3732c16146782e8441d2703934c1215/photo_3_2025-08-09_11-18-05.jpg)

![Image Alt](https://github.com/SNB2025/SNB-SR.-SEC.-SCHOOL/blob/58bbfed6a3732c16146782e8441d2703934c1215/photo_5_2025-08-09_11-18-05.jpg)

![Image Alt](https://github.com/SNB2025/SNB-SR.-SEC.-SCHOOL/blob/58bbfed6a3732c16146782e8441d2703934c1215/photo_7_2025-08-09_11-18-05.jpg)

![Image Alt](https://github.com/SNB2025/SNB-SR.-SEC.-SCHOOL/blob/58bbfed6a3732c16146782e8441d2703934c1215/photo_9_2025-08-09_11-18-05.jpg)




🚀 Goal:
To make school management easier, transparent, and accessible anytime, anywhere—strengthening the bond between school and home.
