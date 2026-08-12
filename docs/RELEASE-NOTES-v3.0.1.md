# WinBoost PRO V3 Enterprise v3.0.1

First public release of WinBoost PRO V3 Enterprise by Tigoor.

## Highlights

- Enterprise Windows diagnostics and Device Diagnostic.
- Network troubleshooting toolkit and Windows Health diagnostics/actions.
- Storage analysis and cleanup, OneDrive / SharePoint diagnostics, and Identity & Access visibility.
- Security & Compliance, Memory Health, Power & Performance, and Startup Apps.
- Custom Script Hub with fixed, approved diagnostics.
- Approved WinGet Software Deployment, trusted Windows Tools, Live Activity, Export Reports, built-in User Guide, and light/dark themes.

## Software Deployment

The approved WinGet catalog includes Google Chrome, Mozilla Firefox, 7-Zip, Visual Studio Code, Notepad++, VLC media player, Microsoft Teams, and Microsoft PowerToys. WinBoost uses fixed approved IDs only, requests confirmation before installation or update, and tracks execution through Live Activity.

## Security & Hardening

The hardened build uses first-party JavaScript obfuscation, ASAR packaging, and a minified PowerShell backend protected by SHA-256 manifest verification. No embedded secrets, source maps, or readable first-party JavaScript are shipped. These controls improve distribution hardening; they do not make reverse engineering impossible.

## Validation

- Core: 128/128 PASS
- Renderer: 30/30 PASS
- Native Electron: 2/2 PASS
- Full bounded: 13/13 PASS
- Portable full-safe: 12/12 PASS
- Script Hub fixtures: 8/8 PASS
- PowerShell parser: 36/36 PASS
- Node syntax: 28/28 PASS
- Authoritative controls: 101; SAFE_AUTO: 65; MANUAL_ONLY: 36
- Automated FAIL: 0; Uncovered: 0; Duplicate IDs: 0; Stale records: 0; Missing activity: 0

## Important: Unsigned Build

This public build is currently unsigned. Windows SmartScreen or Unknown Publisher warnings may appear. Verify SHA-256 before running.

## SHA-256

`012EB43CE953DF77C783D6EB31804897DD6A88F6C314EB1FC000A3942D34FC3D`

## Running

This is a Portable build; no installer is required. Run the executable directly. Administrator Mode is recommended for actions requiring elevation.

## Disclaimer

WinBoost is an IT diagnostics and troubleshooting utility. Disruptive actions require deliberate user interaction or confirmation where applicable. Users remain responsible for testing in their own environment.
