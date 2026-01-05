# Release Notes Template

Use this template when creating a new release on GitHub.

---

## Release Title Format
```
v3.2 - System Checker
```

---

## Release Description (Copy/Paste This)

```markdown
## SecureCheats System Checker v3.2

A free diagnostic tool that scans your Windows PC and generates a comprehensive report for tech support and troubleshooting.

### What's New in v3.2
- Improved GPU driver detection
- Added gaming overlay detection (Discord, Steam, NVIDIA, OBS)
- Better C++ Redistributable scanning
- UI improvements

### Download
Download `SecureCheats_System_Checker.exe` below.

**Requirements:**
- Windows 10 or Windows 11
- Run as Administrator

### Installation
1. Download the .exe file below
2. Right-click → Run as administrator
3. Click "Scan System"

### Antivirus Notice
This tool may trigger false positives in some antivirus software due to being packaged with PyInstaller. It has been verified clean by all major antivirus vendors including Windows Defender, Norton, Kaspersky, and Malwarebytes.

**VirusTotal Scan:** [View Full Report](PASTE_VIRUSTOTAL_LINK_HERE)

### File Verification
```
SHA-256: PASTE_HASH_HERE
```

To verify: Right-click the file → Properties → Digital Signatures, or use `certutil -hashfile SecureCheats_System_Checker.exe SHA256` in Command Prompt.

### Links
- [Website](https://securecheats.com)
- [Tool Page](https://securecheats.com/system-checker/)
- [Installation Help](INSTALLATION.md)
```

---

## How to Create a Release

1. Go to your GitHub repo
2. Click **Releases** (right sidebar)
3. Click **Create a new release**
4. Click **Choose a tag** → type `v3.2` → Create new tag
5. Release title: `v3.2 - System Checker`
6. Paste the description above (edit version numbers, add VirusTotal link, add SHA-256 hash)
7. Drag and drop `SecureCheats_System_Checker.exe` into the attachments area
8. Click **Publish release**

---

## Getting the SHA-256 Hash

Run this in Command Prompt:
```
certutil -hashfile SecureCheats_System_Checker.exe SHA256
```

Or in PowerShell:
```
Get-FileHash SecureCheats_System_Checker.exe -Algorithm SHA256
```

Copy the hash and paste it into the release notes.

---

## Getting the VirusTotal Link

1. Go to [virustotal.com](https://www.virustotal.com)
2. Upload your .exe file
3. Wait for scan to complete
4. Copy the URL from your browser
5. Paste into release notes
