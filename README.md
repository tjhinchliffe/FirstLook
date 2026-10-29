# NAPLAN First Look

Windows downloads for MOSAIC's NAPLAN First Look.

First Look helps educators explore NAPLAN evidence through School Analysis,
Cohort Maps, Cohort Threads and individual Student investigations.

## Windows download

Installers will be available under **Releases** once a Windows build has been
verified and published. No installer has been published yet.

Requirements: Windows 10/11, 64-bit (x64). The installer includes its analysis
runtime; a separate Python installation is not required. Assessment data and
saved investigations remain in the application's configured local storage.
External AI handoff is manual.

Download the `FirstLook-…-Windows-x64-Setup.exe` release asset. Compare its SHA-256
with the accompanying `.sha256` file using PowerShell:

```powershell
Get-FileHash .\FirstLook-<version>-Windows-x64-Setup.exe -Algorithm SHA256
```

Follow your organisation's software approval process. Release notes state whether
an installer is signed and which Windows checks were completed.

This repository is a download centre. Application source, school datasets,
student records, local profiles and development artifacts are not published here.
