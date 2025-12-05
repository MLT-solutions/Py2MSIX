# **How to Use Py2MSIX**

## 📋 Prerequisites
To use this tool, you must have the **Windows 10/11 SDK** installed, specifically:
- `MakeAppx.exe`
- `SignTool.exe`

*These are usually found in `C:\Program Files (x86)\Windows Kits\10\bin\...`*

## 🛠️ How to Use

### Step 1: Prepare your Python App
Compile your script into an executable using PyInstaller:
```bash
pyinstaller --noconsole --onefile --name "MyApp" --icon=app_icon.ico main.py
```

### Step 2: Build the MSIX
* Open Py2MSIX.
* Source: Select your generated .exe (or the dist folder).
* **App Display Name:** This is what users see in the Start Menu (e.g., "Super Calc").
* **Identity Name:** A unique system ID (e.g., "MyCompany.SuperCalc"). No spaces allowed.
* **Publisher:** Must start with `CN=` (e.g., `CN=JohnDoe`). If signing with your own PFX, this **must match** the PFX subject exactly.
* **Version:** Must be in `x.x.x.x` format (e.g., `1.0.0.0`).
* **Custom Logo (PNG):** This part is for the auto-conversion of the logo PNG to two different resolutions.

### Step 3: Store Ready - Signing the Package
* **Use Existing.PFX File:** Select "Self-Signed Certificate" created & include the Password.
* Select Output Location

### Step 4: Build: Click BUILD & SIGN MSIX.

### Troubleshooting
* **"SignTool not found":** Re-install Windows SDK and ensure "Windows App Certification Kit" is selected.
* **"Self-Signed Certificate":** You can Google and find instructions to do this (this is only a temporary signing to upload to Microsoft Store)
