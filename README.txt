NOTELY — COLORFUL NOTES EDITION
================================
A ColorNote-inspired, offline-first notes app for phone and desktop browsers.

FEATURES
- Quick text notes and checklist notes
- Color-coded sticky-note cards
- Grid and list layouts
- Pin notes, search, sort by recent/title/color
- Folders, calendar dates and dated notes
- Trash, restore and permanent deletion
- Duplicate and share/copy notes
- Private notes encrypted locally with AES-GCM and a PIN-derived key
- JSON export and restore (private notes are intentionally excluded)
- Light/dark/system appearance
- Installable PWA and offline cache after the first successful online load

INSTALL / RUN
1. Upload the CONTENTS of this folder to the root of a GitHub Pages repository.
   index.html must be at the repository root, not inside another nested folder.
2. Enable GitHub Pages for the repository and open its HTTPS website in Chrome.
3. Open the browser menu and choose Install app / Add to Home screen.
4. Load once while online so the service worker can cache the app. It can then
   reopen offline in that same browser profile.

DATA & PRIVACY NOTES
- Public notes and folders are stored in IndexedDB in this browser profile.
- This release keeps the previous Notely database name to preserve existing
  public notes when updating from the earlier Notely build.
- Private notes use AES-GCM encryption with a key derived from your PIN.
  Private notes are excluded from ordinary search and backup export.
- If you forget the private PIN, the encrypted notes cannot be recovered.
- Do not clear browser site data or switch browser profiles if you need your notes.
- This is local storage, not cloud sync. Export backups regularly.

LIMITATIONS (IMPORTANT)
- Browser/PWA cannot provide all native Android protections. It cannot guarantee
  hiding the app from Android Recents screenshots or use native biometric unlock.
- Reminder alerts in this build are best-effort while Notely remains open. Browser
  timers may be suspended when the app is closed or the device restarts. Reliable
  background reminders need a native Android app or a supported push service.
- Sharing uses the browser's share sheet when available, otherwise clipboard.
- This is an original Notely interface inspired by common sticky-note workflows;
  it does not include ColorNote's proprietary code, branding or account services.

VERSION
Notely Colorful Notes Edition — 2.0
