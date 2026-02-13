# Kioku

A desktop app for spaced repetition learning with incremental reading.

Kioku combines SuperMemo-style reading workflows with the FSRS scheduling algorithm, so you can import articles, highlight key passages, create flashcards, and review them on an optimized schedule — all offline.

## Download

Go to the [latest release](https://github.com/emrecetintas/kioku-releases/releases/latest) and download the installer for your platform:

| Platform | File | Type |
|----------|------|------|
| **Windows** | `Kioku-x.x.x-x64.exe` | Installer |
| **macOS** | `Kioku-x.x.x-arm64.dmg` | Disk image |
| **Linux** | `Kioku-x.x.x-x86_64.AppImage` | AppImage |
| **Linux (Debian)** | `Kioku-x.x.x-amd64.deb` | Deb package |

Portable `.zip` versions are also available for Windows and macOS.

## Installation Notes

### Windows

On first launch, you may see a SmartScreen warning ("Windows protected your PC"). This is because the app is not yet code-signed. Click **"More info"** then **"Run anyway"**. This only happens once.

### macOS

You may see a Gatekeeper warning ("can't be opened because Apple cannot check it for malicious software"). To open it:

1. Right-click the app and select **Open**
2. Click **Open** in the dialog

Or go to **System Settings > Privacy & Security** and click **"Open Anyway"**.

### Linux

For the AppImage, make it executable first:
```bash
chmod +x Kioku-*.AppImage
./Kioku-*.AppImage
```

For the `.deb` package:
```bash
sudo dpkg -i Kioku-*.deb
```

## Auto-Updates

Kioku checks for updates automatically on launch. When a new version is available, you'll see a banner in the app with a download button. Updates are downloaded in the background and applied on restart.

## Features

- **Incremental reading** — Import articles from the web, read them over time, and extract key passages
- **Spaced repetition** — FSRS-6 scheduling algorithm adapts to your memory
- **Multiple card types** — Basic (front/back), cloze deletions, image occlusion
- **Live imports** — Load pages fresh during review for content that changes
- **Collections** — Separate databases for different subjects or projects
- **Anki import** — Bring your existing decks from Anki (.apkg files)
- **Offline-first** — All data stored locally in SQLite, no account needed
- **Cross-platform** — Windows, macOS, and Linux

## Feedback

Found a bug or have a feature request? Email [kiokufeedback@gmail.com](mailto:kiokufeedback@gmail.com).
