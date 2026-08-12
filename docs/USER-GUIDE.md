# WinBoost PRO V3 User Guide

WinBoost PRO V3 is an offline Windows endpoint-support application. Start the app, allow local diagnostics to initialize, then use the sidebar to select a module. Standard Mode provides available diagnostics; Administrator Mode is required when Windows requires elevation for an action.

## Dashboard and diagnostics

- **Dashboard** summarizes endpoint readiness, device context, resources, findings, and activity.
- **Device Diagnostic** provides local hardware, Windows, firmware, identity, and join information.
- **Network** provides connectivity diagnostics, Ping, DNS Lookup, TCP Port Test, Trace Route, and troubleshooting actions. Disruptive repairs can require confirmation and elevation.
- **Performance** shows CPU, memory, process, and resource-pressure diagnostics.
- **Windows Health** covers Windows integrity, services, updates, printing, security, and available recovery actions.
- **Storage** provides storage health, disk-usage, and safe-cleanup guidance; results are recorded in Live Activity.
- **OneDrive** provides local OneDrive and SharePoint registration diagnostics. It does not modify SharePoint files automatically.
- **Identity & Access** displays local, Entra, and domain identity, device trust, join state, and sign-in readiness.
- **Security & Compliance** provides Defender/security status, Compare Security Status, and a BitLocker management launcher. WinBoost does not replace endpoint security software.
- **Memory Health** includes Refresh Memory, Verify Memory, Task Manager, and Clear Standby Cache. The last action requires confirmation and may require elevation.
- **Power & Performance** displays power-plan information and recovery controls. Sign Out, Sleep, Restart, Shut Down, and Advanced Startup can interrupt the current session.
- **Startup Apps** inventories programs and tasks configured to launch with Windows.

## Custom Script Hub and Software Deployment

Custom Script Hub runs fixed, approved, read-only diagnostics; it is not an arbitrary PowerShell execution surface. Current diagnostic areas are Group Policy, mapped drives, printer drivers, device drivers, Microsoft 365 Apps, user profiles, installed applications, and Outlook / Teams processes.

Software Deployment uses an allow-listed WinGet catalog. WinGet must be available; package IDs cannot be freely entered; confirmation appears before installation or update; and the result is shown in Live Activity. The approved catalog is Google Chrome, Mozilla Firefox, 7-Zip, Visual Studio Code, Notepad++, VLC media player, Microsoft Teams, and Microsoft PowerToys.

## Tools, activity, and reports

Tools opens fixed trusted Windows utilities: Device Manager, Services, Event Viewer, System Information, Credential Manager, Windows Update, Disk Management, Task Manager, Resource Monitor, Terminal, and PowerShell (Admin). It does not accept arbitrary executable paths.

Live Activity has Active, Recent, and Technical Output views. Operations can continue without blocking the whole application, and cancellation appears only where supported.

Export Report can generate HTML, Excel, and CSV endpoint diagnostic and action-history reports.

## Keyboard Shortcuts & Quick Access

No custom application keyboard shortcuts are currently assigned.

The Windows utilities opened from Tools are launcher buttons, not application keyboard shortcuts.

## Safety and troubleshooting

Administrator Mode, confirmations, and MANUAL_ONLY classifications protect disruptive operations. WinBoost does not disable security protections to complete diagnostics, and installation remains restricted to the approved catalog.

If an action is unavailable, check Administrator Mode, Live Activity and Technical Output, network connectivity, and the relevant Windows service or tool. For Software Deployment, verify WinGet health. For Defender, verify Microsoft Defender is available. For OneDrive, verify the local client and account are configured.
