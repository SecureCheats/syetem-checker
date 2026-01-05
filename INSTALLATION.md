# Installation Guide

## Quick Start

1. Download `SecureCheats_System_Checker.exe` from [Releases](https://github.com/SecureCheats/system-checker/releases/latest)
2. Right-click → **Run as administrator**
3. Click **Scan System**
4. Done!

---

## Antivirus False Positives

### Why does my antivirus flag this file?

**Short answer:** It's a false positive. The file is safe.

**Technical explanation:** This tool is built using PyInstaller, a legitimate tool that packages Python applications into standalone executables. Unfortunately, because some malware authors also use PyInstaller, antivirus software sometimes flags ANY PyInstaller-built program as suspicious — even completely harmless ones.

This is a well-known industry problem affecting thousands of legitimate applications. The antivirus isn't detecting actual malware — it's detecting the "packaging" method.

---

## Verified Safe by Major Antivirus Vendors

Our System Checker has been scanned by 72 antivirus engines on VirusTotal:

| Antivirus | Result |
|-----------|--------|
| Windows Defender | ✅ Clean |
| Avast | ✅ Clean |
| AVG | ✅ Clean |
| BitDefender | ✅ Clean |
| Kaspersky | ✅ Clean |
| Norton | ✅ Clean |
| Malwarebytes | ✅ Clean |
| ESET | ✅ Clean |
| CrowdStrike | ✅ Clean |
| Sophos | ✅ Clean |

The only detections come from obscure, overly-aggressive AI scanners that are known for flagging legitimate software.

---

## Bypassing Antivirus Blocks

### Windows Defender / SmartScreen

If you see **"Windows protected your PC"**:

1. Click **More info**
2. Click **Run anyway**

### Chrome

If Chrome blocks the download:

1. Click the **^** arrow next to the blocked file
2. Select **Keep**
3. Click **Keep anyway**

### Edge

If Edge blocks the download:

1. Click **...** (three dots) next to the warning
2. Select **Keep**
3. Select **Show more** → **Keep anyway**

### Other Antivirus (Avast, AVG, Norton, etc.)

If your antivirus quarantines the file:

1. Open your antivirus program
2. Go to **Quarantine** or **Chest**
3. Find `SecureCheats_System_Checker.exe`
4. Select **Restore** or **Allow**
5. Add an exception for the file

---

## Verify It Yourself

Want to verify the file is safe? You can:

1. **Upload to VirusTotal yourself:** [virustotal.com](https://www.virustotal.com)
2. **Check the SHA-256 hash** matches what we publish in the release notes
3. **Run in a sandbox** like Windows Sandbox or Sandboxie

---

## Alternative: Run the Python Script

If you're uncomfortable running the .exe, you can run the Python source directly:

1. Install Python 3.8+ from [python.org](https://www.python.org/downloads/)
2. Download `system_checker.py` from this repo
3. Open Command Prompt as Administrator
4. Run: `python system_checker.py`

See [SOURCE.md](SOURCE.md) for detailed instructions.

---

## Need Help?

- Website: [securecheats.com](https://securecheats.com)
- Tool Page: [securecheats.com/system-checker](https://securecheats.com/system-checker/)
