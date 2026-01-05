# Running from Source Code

If you prefer to run the Python script directly instead of the .exe, follow these instructions.

## Why Run from Source?

- **Full transparency** — You can inspect every line of code
- **No antivirus issues** — Python scripts don't trigger false positives
- **Modify it yourself** — Customize the tool for your needs

---

## Requirements

- Python 3.8 or higher
- Windows 10 or Windows 11
- Administrator privileges (for full system access)

---

## Installation

### Step 1: Install Python

1. Download Python from [python.org](https://www.python.org/downloads/)
2. Run the installer
3. **Important:** Check "Add Python to PATH" during installation
4. Click Install

### Step 2: Download the Script

Download `system_checker.py` from this repository.

### Step 3: Install Dependencies

Open Command Prompt as Administrator and run:

```
pip install wmi pywin32
```

### Step 4: Run the Script

```
python system_checker.py
```

---

## Dependencies

| Package | Purpose |
|---------|---------|
| `wmi` | Windows Management Instrumentation queries |
| `pywin32` | Windows API access for registry and system info |

Both are well-known, trusted packages available on PyPI.

---

## Building the .exe Yourself

If you want to compile your own executable:

### Step 1: Install PyInstaller

```
pip install pyinstaller
```

### Step 2: Build

```
pyinstaller --onefile --windowed system_checker.py
```

The .exe will be in the `dist` folder.

### Optional: Custom Icon

```
pyinstaller --onefile --windowed --icon=icon.ico system_checker.py
```

---

## Code Overview

The script uses standard Windows APIs to gather system information:

| Function | What it checks |
|----------|----------------|
| `get_os_info()` | Windows version, build, activation |
| `get_hardware_info()` | Motherboard, BIOS, RAM via WMI |
| `get_gpu_info()` | GPU model, driver version, driver date |
| `get_security_info()` | Secure Boot, TPM, BitLocker via registry |
| `get_antivirus_info()` | Security Center WMI queries |
| `get_runtime_info()` | Registry scan for C++, DirectX DLLs |
| `get_overlay_info()` | Process list and registry checks |

---

## Questions?

- Website: [securecheats.com](https://securecheats.com)
- Tool Page: [securecheats.com/system-checker](https://securecheats.com/system-checker/)
