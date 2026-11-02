# NAPLAN First Look

Windows and macOS downloads for MOSAIC's NAPLAN First Look.

First Look helps educators explore NAPLAN evidence through School Analysis,
Cohort Maps, Cohort Threads and individual Student investigations.

## Downloads — 2027.0.1 preview

| Computer | Download | Requirements |
| --- | --- | --- |
| Windows PC | [Windows x64 installer](https://github.com/tjhinchliffe/FirstLook/releases/download/v2027.0.1-preview.1/FirstLook-2027.0.1-Windows-x64-Setup.exe) | Windows 10/11, 64-bit |
| Mac with Apple Silicon (M1 or later) | [macOS Apple Silicon disk image](https://github.com/tjhinchliffe/FirstLook/releases/download/v2027.0.1-preview.1/FirstLook-2027.0.1-macOS-arm64.dmg) | macOS 15 or later |
| Mac with an Intel processor | [macOS Intel disk image](https://github.com/tjhinchliffe/FirstLook/releases/download/v2027.0.1-preview.1/FirstLook-2027.0.1-macOS-x64.dmg) | macOS 15 or later |

[Release notes and SHA-256 checksum files](https://github.com/tjhinchliffe/FirstLook/releases/tag/v2027.0.1-preview.1)

To check your Mac's processor, open **Apple menu → About This Mac**. Choose
Apple Silicon if it lists a Chip such as Apple M1, M2, M3 or later; choose Intel
if it lists an Intel processor.

On macOS, open the downloaded DMG and drag **NAPLAN First Look** into
**Applications**, then eject the disk image and launch from Applications.
Each download includes the native analysis worker and offline report renderer;
no separate Python installation is required.

These are **preview packages**. The Windows installer is unsigned. The Mac apps
are ad-hoc signed, but are **not Apple Developer ID signed or notarized**.
macOS or your school's device policy may block them or require IT approval.
Follow your organisation's software approval process before installation.

## Verification

Both Mac disk images were mounted and their exact packaged apps tested on native
Apple Silicon and Intel macOS runners. Checks cover offline synthetic-source
import, all four main views, restart persistence, Help, the external Training
Guide, and Excel, Word, HTML and PDF exports with system Python disabled.
The app signatures were checked before and after use.

The existing Windows EXE was installed and tested on a Windows runner, including
offline import, all four main views, restart and the Training Guide browser link
with system Python disabled. Its download is unchanged by this Mac release.

Physical managed-device, display-scaling and assistive-technology checks remain
separate from these automated checks.

## Check your download

Compare the downloaded file's SHA-256 with its accompanying `.sha256` release
asset. On macOS, use Terminal with the actual downloaded filename:

```sh
shasum -a 256 ~/Downloads/FirstLook-2027.0.1-macOS-arm64.dmg
```

For Intel Macs, replace `arm64` with `x64`. On Windows, use PowerShell:

```powershell
Get-FileHash .\FirstLook-2027.0.1-Windows-x64-Setup.exe -Algorithm SHA256
```

Assessment data and saved investigations remain in the application's configured
local storage. External AI handoff is manual.

This repository is a download centre. Application source, school datasets,
student records, local profiles and development artifacts are not published here.
