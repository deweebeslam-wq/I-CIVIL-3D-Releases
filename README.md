# i-CIVIL for Civil 3D

[![Latest release](https://img.shields.io/github/v/release/deweebeslam-wq/I-CIVIL-3D-Releases?style=flat-square&color=2B5797)](https://github.com/deweebeslam-wq/I-CIVIL-3D-Releases/releases/latest)
![Civil 3D](https://img.shields.io/badge/Civil%203D-2026-0696D7?style=flat-square&logo=autodesk&logoColor=white)
![Navisworks plugin](https://img.shields.io/badge/Navisworks%20plugin-2025-D97B1E?style=flat-square)
![Platform](https://img.shields.io/badge/Windows-x64-0078D6?style=flat-square&logo=windows&logoColor=white)

**Importers, pipe network tools, Navisworks link, BIM and sheet export and a Smart Filter in one Civil 3D ribbon tab** —
built by [I-BIMS](https://github.com/deweebeslam-wq), the makers of [I-TOOLS for Revit](https://github.com/deweebeslam-wq/I-TOOLS-Releases) and [I-TOOLS for Navisworks](https://github.com/deweebeslam-wq/I-TOOLS-NAVIS-Releases).

This repository hosts the **installers** and the `update.json` files that i-CIVIL's built-in
updater reads. The source code is private.

## Download

**[⬇ Latest release](https://github.com/deweebeslam-wq/I-CIVIL-3D-Releases/releases/latest)** → download `iCIVIL-Setup-<version>.exe`, close Civil 3D and run it.

- Choose **all users** (Windows asks for administrator permission) or **just me** (no admin rights needed)
- The optional **Navisworks plugin** adds *Send to Civil 3D* to the right-click menu in Navisworks Manage and Simulate 2025
- Civil 3D loads the add-in by itself the next time it starts — look for the **i-CIVIL** ribbon tab
- Windows may show a SmartScreen warning because the installer is not yet code-signed: *More info → Run anyway*

## Updates

Install **1.9.0 or later** once — after that i-CIVIL **updates itself**:

- About 20 seconds after Civil 3D starts, i-CIVIL checks this repository (at most once a day)
- If a newer version exists you see what's new and choose **Update Now** or **Later**
- Every download is checked against its **SHA-256** before anything is installed; a failed or cancelled install leaves your current version untouched
- Civil 3D keeps the add-in files in use, so the update **installs as soon as you close Civil 3D** — the i-CIVIL updater waits in its own small window
- **i-CIVIL ▸ Updates** (`ICIVILUPDATES`): check now, choose *Ask me before installing* or *Download automatically*, or opt in to beta versions

## What's inside

| Panel | Tools |
|---|---|
| **Importers** | Import Points (CSV, TXT, Excel) · Blocks to Points · Import LandXML · Import Pipe Network · Import Profile |
| **Pipes** | Lines to Pipes · Structures from Points · Points on Structures · Pipe Editor · Structure Editor · Split Pipe · Set Pipe Cover · Level Services · Swap Parts · Pipe Elevation · Part Properties · Structure Reference · Structure Report |
| **Navisworks** | Find by Handle · Copy Handle · Navis > Acad (3D blocks from a Navisworks selection at exact coordinates) |
| **BIM Export** | Navisworks NWC and IFC from one dialog, by category, network, surface, block, layer or picked objects |
| **Sheets** | Sheet Export: one PDF per layout, a combined PDF and plain AutoCAD DWGs, in the background |
| **Selection** | Smart Filter (`SFILTER`): find objects by type and any mix of property rules, then select, zoom to, isolate, hide or export them |

Release notes for every version are on the **[Releases](https://github.com/deweebeslam-wq/I-CIVIL-3D-Releases/releases)** page.

## Troubleshooting

| Problem | What to do |
|---|---|
| The i-CIVIL tab doesn't appear | Restart Civil 3D after installing. i-CIVIL loads only in Civil 3D 2026 |
| The setup says i-CIVIL is in use | Close Civil 3D (or Navisworks, for the plugin) and click **Retry** |
| The update never installs | Close Civil 3D and check Task Manager for `acad.exe` and `accoreconsole.exe` — plus `Roamer.exe` if the Navisworks plugin is installed. The i-CIVIL updater installs as soon as they are gone |
| "Windows did not get administrator permission" | The update was not installed. Use **i-CIVIL ▸ Updates ▸ Check for Updates** again and click **Yes** when Windows asks |
| Anything else | Send `%LOCALAPPDATA%\i-CIVIL\logs\Updater.log` (and the latest `iCIVIL-*.log` from the same folder) with an [issue](https://github.com/deweebeslam-wq/I-CIVIL-3D-Releases/issues) |

---

© I-BIMS · Eslam Deweeb. All rights reserved.
