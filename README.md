# Py2MSIX - Python to App Store Packager
A simple solution to compile exe &amp; sign it into MSIX format for MS Store submission

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Platform](https://img.shields.io/badge/platform-Windows-blue) ![Python](https://img.shields.io/badge/python-3.x-yellow)

A streamlined GUI tool to package Python applications (and other executables) into MSIX packages ready for the Microsoft Store or sideloading.

## 🚀 Features
- **Visual Interface:** No more memorizing `MakeAppx` command line arguments.
- **Auto-Signing:** Creates and applies self-signed certificates for testing.
- **Asset Resizing:** Takes one high-res logo and generates all required Store icons.
- **Folder Support:** Package entire directories (great for PyInstaller `--onedir` builds).

| Feature | Manual CLI Method | Py2MSIX | 
| :--- | :--- | :--- | 
| Manifest Creation | Hand-edit complex XML | Visual Form Fill | 
| Image Resizing | Manually resize 3+ PNGs | Auto-Resize | 
| Certificate Creation | 3-step PowerShell commands | 1-Click Auto | 
| Learning Curve | High (Docs & Syntax) | Zero |



🤝 Contributing
Found a bug? Open an Issue. Want a feature? Vote on existing issues or create a PR!
https://github.com/MLT-solutions/Py2MSIX/issues
