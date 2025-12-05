# Help Menu Guide (General Usage)

**How to Use Py2MSIX**

**1. Prerequisites**
Before starting, please make sure you have the **Windows 10/11 SDK** installed. This provides the necessary packing tools (`MakeAppx` and `SignTool`).

**2. Preparing Your App**
Py2MSIX packages existing executables. First, compile your Python script:
* **Command:** `pyinstaller --noconsole --onefile --name "MyApp" --icon=app.ico main.py`
* *Tip:* Use `--onefile` for simpler packaging, or select "Browse Folder" in Py2MSIX if you have many dependency files.

**3. Configuration Fields**
* **App Display Name:** This is what users see in the Start Menu (e.g., "Super Calc").
* **Identity Name:** A unique system ID (e.g., "MyCompany.SuperCalc"). No spaces allowed.
* **Publisher:** Must start with `CN=` (e.g., `CN=JohnDoe`). If signing with your own PFX, this **must match** the PFX subject exactly.
* **Version:** Must be in `x.x.x.x` format (e.g., `1.0.0.0`).
* **Custom Logo (PNG):** This part is for the auto-conversion of the logo PNG to two different resolutions.

**4. Store Ready - Signing the Package**
* **Use Existing.PFX File:** Select "Self-Signed Certificate" created & include the Password.

**5. Troubleshooting**
* **"SignTool not found":** Re-install Windows SDK and ensure "Windows App Certification Kit" is selected.
* **"Self-Signed Certificate":** You can Google and find instructions to do this (this is only a temporary signing to upload to Microsoft Store)
