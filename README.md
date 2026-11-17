# Blinkshare Releases

Official download repository for **Blinkshare** — ultra-fast, direct peer-to-peer file sharing and local network streaming.

[![Release](https://img.shields.io/github/v/release/De-Hype/blinkshare-releases?style=flat-square&color=blue)](https://github.com/De-Hype/blinkshare-releases/releases/latest)
[![Platform](https://img.shields.io/badge/platform-macOS%20%7C%20Windows%20%7C%20Linux-lightgrey?style=flat-square)](#download)
[![License](https://img.shields.io/badge/license-Proprietary-blue?style=flat-square)](#)

---

## 📥 Download

Download the latest version directly from the [Latest Releases](https://github.com/De-Hype/blinkshare-releases/releases/latest) page:

| Operating System | Architecture | Installer / Package |
| :--- | :--- | :--- |
| 🍏 **macOS (Apple Silicon)** | M1 / M2 / M3 / M4 (`arm64`) | [**Download .dmg**](https://github.com/De-Hype/blinkshare-releases/releases/latest) \| [Download .zip](https://github.com/De-Hype/blinkshare-releases/releases/latest) |
| 🍏 **macOS (Intel)** | x86_64 (`x64`) | [**Download .dmg**](https://github.com/De-Hype/blinkshare-releases/releases/latest) \| [Download .zip](https://github.com/De-Hype/blinkshare-releases/releases/latest) |
| 🪟 **Windows** | 64-bit (`x64`) | [**Download Setup .exe**](https://github.com/De-Hype/blinkshare-releases/releases/latest) \| [Standalone .exe](https://github.com/De-Hype/blinkshare-releases/releases/latest) |
| 🐧 **Linux (Universal)** | 64-bit (`x86_64`) | [**Download .AppImage**](https://github.com/De-Hype/blinkshare-releases/releases/latest) |
| 🐧 **Linux (Debian / Ubuntu)** | 64-bit (`amd64`) | [**Download .deb**](https://github.com/De-Hype/blinkshare-releases/releases/latest) |

---

## 🍏 macOS Installation Guide

If macOS displays the warning:
> **“Blinkshare” cannot be opened because the developer cannot be verified.**  
> *macOS cannot verify that this app is free from malware.*

This occurs because Blinkshare is built directly from source and is not yet signed with an Apple Developer Program certificate.

### How to Open on macOS:
* **Option 1 (Quickest):**
  1. Locate `Blinkshare.app` in Finder (or your `/Applications` folder).
  2. **Right-click** (or hold **Control** and click) on `Blinkshare.app`.
  3. Click **Open** in the context menu.
  4. In the dialog box that appears, click the **Open** button. *(You only need to do this once).*
* **Option 2 (System Settings):**
  1. Open **System Settings** > **Privacy & Security**.
  2. Scroll down to **Security**.
  3. Look for the message: *"Blinkshare was blocked from use because it is not from an identified developer"*.
  4. Click **Open Anyway**.
* **Option 3 (Terminal):**
  ```bash
  xattr -cr /Applications/Blinkshare.app
  ```

---

## 🐧 Linux Installation Guide

### AppImage
Make the downloaded `.AppImage` executable and run it:
```bash
chmod +x Blinkshare-*-x86_64.AppImage
./Blinkshare-*-x86_64.AppImage
```

### Debian / Ubuntu (.deb)
Install using `dpkg` or `apt`:
```bash
sudo dpkg -i Blinkshare-*_amd64.deb
sudo apt-get install -f # Fix any missing dependencies if needed
```

---

## 🔒 Verification & Checksums

Each release includes a `checksums.txt` file containing SHA-256 hashes for all downloadable files.

To verify a downloaded file on macOS / Linux:
```bash
shasum -a 256 <filename>
```
On Windows (PowerShell):
```powershell
Get-FileHash <filename> -Algorithm SHA256
```

---

© 2026 [Blinkshare](https://github.com/De-Hype). All rights reserved.
