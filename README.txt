NOTELY V1.0 — PHONE-ONLY SETUP

WHAT'S INCLUDED
- Notes with six page styles and colors
- Checklists with completion tracking
- Custom note/checklist icons
- Folders
- Monthly calendar with date-linked notes
- Private notes encrypted with AES-GCM using a PIN-derived key
- Grid/list view, light/dark/system theme
- Local JSON backup and restore
- IndexedDB local storage and offline service worker

IMPORTANT LIMITATIONS
- This is a first PWA build, not a native Android APK.
- For install/offline support, host the files on HTTPS (GitHub Pages is a free option).
- Private note data is encrypted in IndexedDB. The PIN cannot be reset; if forgotten, private notes cannot be decrypted.
- Biometrics and Android recent-app screenshot blocking require native Android packaging and are not available in this PWA build.
- Export backup currently exports regular notes and folders. Private notes are intentionally excluded so they are not accidentally exported in plaintext.

INSTALL USING ONLY YOUR PHONE
1. Extract notely-v1.zip on your phone.
2. Create a free GitHub repository named notely (or another name).
3. Upload the CONTENTS of this folder to the repository root (index.html must be at the root).
4. In the repository, open Settings > Pages.
5. Select Deploy from a branch, choose main and /(root), then Save.
6. Wait for GitHub Pages to publish. Open the published HTTPS address in Chrome.
7. Use Chrome menu (⋮) > Add to Home screen or Install app.
8. Open Notely once while online so the service worker caches the app. Then test airplane mode.

TESTING
- Notes and folders are saved in the browser's IndexedDB on this device.
- Clearing Chrome site data may erase your notes. Export regular-note backups periodically.
- Use the same browser profile and published address to access your data.

PROJECT FILES
index.html       App interface
styles.css       Visual design
app.js           Notes, folders, calendar, privacy and backup logic
manifest.webmanifest  Installable app metadata
sw.js            Offline app-shell cache
icons/           App icons
