# 📖 HDO PRO Wiki

General guides and educational resources about Android, sideloading, and device security.

> **Looking for HDO PRO downloads?** You won't find them here. This repository does not host or link to HDO PRO APKs, builds, or download files.

---

# 📌 Purpose

This wiki provides general Android information. It is not a download center, support portal, or installation guide for HDO PRO.

---

# 📲 ANDROID SIDELOADING GUIDE

<details>
<summary>Quick Steps</summary>

### Android Phone/Tablet
1. **Enable Unknown Sources:** Settings > Security > Install unknown apps (allow for your browser)
2. **Download APK** from trusted source
3. **Open file** from Downloads
4. **Tap Install**
5. **Launch app** when complete

### Android TV / Google TV
1. **Install Downloader app** from Google Play Store
2. **Enable Unknown Sources:** Settings > Security & restrictions > Install unknown apps > Allow Downloader
3. **Open Downloader** and enter URL or download code
4. **Install APK** when download completes
5. **Delete APK** after installation

### Fire TV / Fire Stick
1. **Enable Developer Options:** Settings > My Fire TV > About > Click Fire TV 7x
2. **Install Downloader** from Amazon Appstore
3. **Enable Apps from Unknown Sources:** Settings > My Fire TV > Developer Options
4. **Open Downloader** and enter URL or code
5. **Install** and delete APK

### Safety Tips
- Scan APKs with [VirusTotal](https://www.virustotal.com) before installing
- Only download from trusted sources
- Disable Unknown Sources after installation
- Keep device updated
- Use [Android Toolkit](https://github.com/AnthonyGress/Android-Toolkit) for safer ADB-based installations
- Backup important data before modifying system settings

</details>

---

# � ADB CONNECTION TROUBLESHOOTING

<details>
<summary>Common Issues</summary>

### Can't connect via ADB
- **Device not found:** Ensure ADB debugging is enabled
- **Connection refused:** Check both devices are on same network
- **Unauthorized:** Accept debugging prompt on device
- **Firewall blocking:** Allow ADB through firewall
- **Wrong IP:** Verify device IP address in settings

### Fire TV Specific
- Enable ADB Debugging: Settings > My Fire TV > Developer Options > ADB Debugging
- Enable Apps from Unknown Sources: Settings > My Fire TV > Developer Options > Apps from Unknown Sources
- Find IP: Settings > My Fire TV > About > Network

### Android TV Specific
- Enable USB Debugging: Settings > Device Preferences > About > Build Number (tap 7x) > Developer Options > USB Debugging
- Enable Network Debugging: Developer Options > Network ADB Debugging

</details>

---

# � XAPK INSTALLER GUIDE

For information about XAPK installers, see the **HDO PRO XAPK Installer Guide** repository.

**Includes:**
- Recommended XAPK installers
- What XAPK files are
- Installation best practices
- Android package formats
- Safety recommendations

> The XAPK Installer Guide is informational only. It does not contain HDO PRO downloads, APKs, XAPKs, source code, or installation packages.

---

# 🛡️ STAY SAFE

**Good security habits:**
- Download only from trusted sources
- Avoid unknown or modified APKs
- Check file names and versions
- Use Google Play Protect
- Keep Android updated

If something doesn't feel right, don't install it.

---

# 🛠️ RECOMMENDED TOOLS

## [HDO PRO Android System Toolkit](https://github.com/HDO-PRO/android-system-toolkit)

Community toolkit for Android device management and system utilities.

## [Android Toolkit](https://github.com/AnthonyGress/Android-Toolkit)

A cross-platform desktop app for managing Android devices via ADB. Useful for:
- **APK Installation:** Single APK install, batch install, quick install popular apps
- **TV Apps:** SmartTube (ad-free YouTube), Launcher Manager, Wolf Launcher (block ads)
- **Mobile Apps:** ReVanced (modded YouTube, Reddit, Spotify)
- **FireTV Tools:** Custom screensaver, debloat (remove Amazon bloatware)
- **System Tools:** Device management, debugging

**Download:** [Android-toolkit-setup.exe](https://github.com/AnthonyGress/Android-Toolkit/releases/latest/download/Android-toolkit-setup.exe)

## Useful Utility Apps
- **[SmartTubeNext](https://github.com/yuliskov/SmartTubeNext)** - Ad-free YouTube for Android TV
- **[Wolf Launcher](https://www.techdoctoruk.com/tutorials/block-android-tv-adverts-with-wolf-launcher/)** - Block Android TV ads
- **[ReVanced](https://revanced.app/)** - Modded apps (YouTube, Reddit, Spotify)
- **[Activity Launcher](https://www.f-droid.org/en/packages/de.szalkowski.activitylauncher/)** - Launch hidden system activities

---

# �� SCAN FILES BEFORE INSTALLING

Before opening an APK, consider scanning with:
- [VirusTotal](https://www.virustotal.com)
- [Hybrid Analysis](https://www.hybrid-analysis.com)
- [MetaDefender Cloud](https://metadefender.com)
- [Google Play Protect](https://play.google.com/store)

No scanner can guarantee a file is completely safe.

---

# ❌ COMMON SIDELOADING ERRORS & FIXES

<details>
<summary>Error Solutions</summary>

### Parse Error
- **Cause:** APK incompatible with device architecture or corrupted download
- **Fix:** Re-download APK, check device compatibility (arm64-v8a, armeabi-v7a)

### Installation Failed
- **Cause:** Insufficient storage, conflicting app, or signature mismatch
- **Fix:** Clear storage, uninstall existing version, disable Play Protect temporarily

### App Not Installed
- **Cause:** Unknown sources disabled or package signature conflict
- **Fix:** Enable unknown sources, uninstall existing app with same package name

### Blocked by Play Protect
- **Cause:** Google security flagging
- **Fix:** Tap "Install anyway" or temporarily disable Play Protect

### Certificate Mismatch
- **Cause:** Installing modded app over original
- **Fix:** Uninstall original app first, then install modded version

### Download Failed
- **Cause:** Network issues or server down
- **Fix:** Check internet connection, try alternative download source

</details>

---

# 🔍 APK VERIFICATION DETAILS

**How to verify APK integrity:**
- **Check file size:** Compare with expected size from source
- **Verify hash:** Use SHA-256 checksum if provided
- **Check signature:** Verify app signature matches original
- **Package name:** Confirm package name is expected (e.g., com.example.app)
- **Version info:** Verify version code and name

**Using apksigner (advanced):**
```bash
apksigner verify --print-certs your-app.apk
```

**Using keytool (advanced):**
```bash
keytool -printcert -jarfile your-app.apk
```

---

# 🌍 INTERNET & PRIVACY

**When downloading:**
- Use stable internet connection
- Avoid public Wi-Fi when possible
- Consider using a reputable VPN on untrusted networks
- A trusted DNS provider may improve privacy

VPN and DNS are privacy tools, not malware protection.

---

# � APP PERMISSIONS GUIDE

**Permissions to watch out for:**
- **Phone/SMS:** Unnecessary for streaming apps
- **Contacts:** Not needed for media apps
- **Location:** Only needed if app has local content
- **Camera/Microphone:** Suspicious for streaming apps
- **Read/Write Storage:** Normal for downloading content

**Red flags:**
- Requesting admin/root access
- Requesting accessibility service
- Requesting device admin privileges
- Excessive permissions for app function

**Best practices:**
- Review permissions before installing
- Deny unnecessary permissions if possible
- Use apps with minimal permission requirements
- Research app reputation if permissions seem excessive

---

# � STORAGE MANAGEMENT TIPS

**Free up space before installing:**
- Clear app cache: Settings > Apps > Select app > Storage > Clear Cache
- Delete unused apps and games
- Remove downloaded videos/files from Downloads
- Move photos/videos to cloud storage or computer
- Clear system cache (requires reboot or recovery mode)

**For Fire TV / Android TV:**
- Uninstall unused apps from Settings > Applications
- Clear cache for streaming apps regularly
- Use external storage if device supports it
- Remove downloaded content from apps after watching

**General tips:**
- Keep at least 1GB free for app installations
- Larger apps (games) may need 2-3GB free space
- APK files can be deleted after installation
- Some apps cache content that grows over time

---

# �📦 BEFORE INSTALLING

Always verify:
- ✅ File comes from trusted source
- ✅ Version is what you expect
- ✅ File has been scanned
- ✅ Device has enough storage
- ✅ Internet connection is stable

---

# ❓ LOOKING FOR HDO PRO?

This repository intentionally contains:
- ❌ No HDO PRO downloads
- ❌ No APK files
- ❌ No XAPK files
- ❌ No source code
- ❌ No release builds
- ❌ No installation packages
- ❌ No hidden download links

Nothing here provides access to HDO PRO.

---

# ⚖️ DISCLAIMER

This wiki is a collection of general Android knowledge and security guidance. It is not a source for HDO PRO software, downloads, community access, or installation packages.

---

<div align="center">

# 📖 HDO PRO Wiki

**Knowledge is here. Downloads are not.**

</div>
