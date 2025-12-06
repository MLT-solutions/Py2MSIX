# Py2MSIX - Python to App Store Packager
A simple solution to compile exe &amp; sign it into MSIX format for MS Store submission

![Platform](https://img.shields.io/badge/platform-Windows-blue) ![Python](https://img.shields.io/badge/python-3.x-yellow)


<img width="1479" height="795" alt="Screenshot 2025-12-06 093635" src="https://github.com/user-attachments/assets/af3c3f61-cbff-4b27-b980-18504226f324" />



A streamlined GUI tool to package Python applications (and other executables) into MSIX packages ready for the Microsoft Store or sideloading.

## Details:

If you have a Python script or executable, you are 90% of the way to the Microsoft Store. Py2MSIX bridges that final 10% gap. It wraps your code into a compliant MSIX package, handles the manifest creation, and even signs it for you—all from a simple dashboard.

### **🌟 Master Feature List**

* **Visual Manifest Editor:** Forget about hand-editing AppxManifest.xml. Input your Publisher Name, Version, and Identity in a clean GUI.  
* **One-Click Packaging:** Instantly converts your Python .exe or entire project directories (great for PyInstaller \--onedir builds) into a deployable .msix.  
* **Smart Asset Generator:** Upload a single high-quality logo, and the app automatically resizes it to the required Store formats (44x44, 150x150, and Store Logo).  
* **Live Diagnostics:** View real-time build logs to troubleshoot MakeAppx or SignTool errors instantly without leaving the app.


**🆚 Comparison Table (The "Why")**

| Feature | Manual CLI Method | Py2MSIX |
| :---- | :---- | :---- |
| **Manifest Creation** | Hand-edit complex XML files | **Visual Form Fill** |
| **Image Handling** | Manually resize & rename 3+ PNGs | **Auto-Resize from 1 Image** |
| **Learning Curve** | High (Requires Docs & Syntax) | **Zero** |


🤝 Contributing
Found a bug? Open an Issue. Want a feature? Vote on existing issues or create a PR!

https://github.com/MLT-solutions/Py2MSIX/issues
