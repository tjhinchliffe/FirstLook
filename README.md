# NAPLAN First Look

Windows downloads for MOSAIC's NAPLAN First Look.

First Look helps educators explore NAPLAN evidence through School Analysis,
Cohort Maps, Cohort Threads and individual Student investigations.

## Windows download

[Download the Windows x64 installer](https://github.com/tjhinchliffe/FirstLook/releases/download/v2027.0.1-preview.1/FirstLook-2027.0.1-Windows-x64-Setup.exe)

[Release notes and SHA-256 checksum](https://github.com/tjhinchliffe/FirstLook/releases/tag/v2027.0.1-preview.1)

The current download is an **unsigned Windows preview**. The exact EXE was
installed and tested on a Windows runner, including offline import, the four main
views, restart and the Training Guide browser link with system Python disabled.
Physical managed-device, display-scaling and assistive-technology checks remain
separate from these automated checks.

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
