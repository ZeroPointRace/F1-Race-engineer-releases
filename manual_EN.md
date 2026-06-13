# F1 Race Engineer — User Manual

> **Game:** EA Sports F1 25 (base + 2026 Season Pack DLC) · **Version:** see the bottom-left corner of the main menu
> **Support:** f1zeropointracing@gmail.com · **Community:** [Discord](https://discord.gg/fbRscvmJtV)

---

## Table of Contents

1. [Installation](#1-installation)
2. [First launch and license](#2-first-launch-and-license)
3. [Entering a license key](#3-entering-a-license-key)
4. [Configuring F1 25](#4-configuring-f1-25)
5. [Using it during a race](#5-using-it-during-a-race)
6. [Troubleshooting](#6-troubleshooting)
7. [Security and privacy](#7-security-and-privacy)

---

## 1. Installation

### System requirements

| Component | Minimum |
|---|---|
| Operating system | Windows 10 64-bit (or newer) |
| RAM | 4 GB |
| Processor | Any x64 CPU from 2015 or later |
| Network | Internet connection (for license activation and first launch) |
| Game | EA Sports F1 25 (PC) |

### Downloading the installer

The installer, always the latest version, is available here:

👉 **https://github.com/ZeroPointRace/F1-Race-engineer-releases/releases/latest**

1. Open the link above
2. Under **"Assets"**, click the `F1-Race-Engineer-Setup-x.y.z.exe` file
3. If your browser warns it's "not safe", click **Save** / **Keep** — the file is safe, it just isn't (paid) code-signed

### Installation

The installer is **one-click**: no wizard, no folder selection.

1. Run the downloaded `.exe`
2. If Windows SmartScreen appears → **"More info"** → **"Run anyway"**
3. The app **installs and launches automatically** (into your user folder, no admin rights needed) and creates a desktop + Start menu shortcut named **"F1 Race Engineer"**

> 💡 You only need the link above for the **first** install. After that the app **updates automatically** (see section 6) — it downloads and offers new versions on its own.

---

## 2. First launch and license

### Starting the app

Double-click the **F1 Race Engineer** desktop shortcut. The intro splash appears, followed by the main menu.

> The engine (backend) starts automatically in the background; on the first launch this takes a few seconds. Don't close the window while it loads.

### Trial (free trial period)

If you don't have a paid license key yet, the app automatically starts a **14-day trial**. No activation needed, it works immediately.

During the trial all features are available; the main menu shows how many days are left.

**After the trial expires** the app runs in restricted mode (only the settings pages are available), with no race support — you then need to enter a license key.

---

## 3. Entering a license key

### Getting a key

You can request a key from the **License** page in the app (enter your email — you get a key by email), or from the developer (f1zeropointracing@gmail.com). Key format: `XXXXX-XXXXX-XXXXX-XXXXX`.

### Activation steps

1. Open the app
2. In the main menu click **"License"**
3. Type the key into the field (with or without dashes — doesn't matter)
4. Click **"Activate"**
5. If you're online and the key is valid → **"License activated"** appears

> Activation binds the key to this machine (based on a hardware ID), and the validity period starts from the moment of activation. To move it to a new machine, contact us by email.

### What the license page shows

| Status | Meaning |
|---|---|
| ✅ Active | All features available |
| ⏳ Trial (N days left) | Trial period, all features available |
| ❌ Expired | Trial or license expired — enter a key |
| 🔒 Revoked | The key was invalidated (e.g. due to misuse) |
| 📡 Offline | No internet, but the 7-day grace period is active — everything works |

---

## 4. Configuring F1 25

F1 Race Engineer listens to the game's UDP telemetry stream. This needs to be set up once.

### Enabling telemetry in F1 25

1. Start F1 25
2. Go to: **Settings → Telemetry Settings**
3. Set the following:

| Setting | Value |
|---|---|
| UDP Telemetry | **On** |
| UDP IP Address | `127.0.0.1` (if you play on the same PC) |
| UDP Port | **20777** |
| UDP Send Rate | **20Hz** or **60Hz** |
| UDP Format | **2025** (base) or **2026** (with the 2026 Season Pack DLC) |
| Your Telemetry | **Public** |

> 💡 The main menu shows your **PC IP** with a **📋 copy** button — paste it into the game's UDP IP Address field. If you stream the game from a console to PC (Remote Play), the IP is the console's network IP, not `127.0.0.1` — contact us in that case.

### Configuring the app

1. In the main menu click **"Race settings"**
2. Set:
   - **Strategy mode:** Auto (recommended) or Manual
   - **Mandatory pit stops / tyre rules** (for league racing)
   - **Audio:** language and voice
3. Click **"Save settings"** — you return to the main menu

> Settings are stored on your machine; you don't need to re-enter them next time.

---

## 5. Using it during a race

### Before the race

1. Start **F1 Race Engineer**
2. Start **F1 25** (order doesn't matter, but launching F1 RE first is recommended)
3. Enter the race menu — the app automatically detects the session and switches to the right view

### Main menu buttons

| Button | Function |
|---|---|
| **Race** | Opens the live dashboard |
| **Race settings** | Strategy and audio settings |
| **Wheel commands** | Voice queries bound to wheel buttons |
| **Language** | Hungarian / English switch |
| **License** | License key management |

### The Dashboard (live race view)

The Dashboard opens automatically when F1 25 detects a race. It shows:
- **Position** and gap to the car ahead / behind
- **Tyre state** (wear %, temperature — blue=cold, green=optimal, red=overheated)
- **ERS level** and usage
- **Wind and weather forecast**
- **SC/VSC status** (yellow bar when a Safety Car is active)
- **Decision suggestions** — what the engineer says also appears here as text

### What the engineer's voice messages mean

The app talks to you during the race in **Hungarian** (or English, depending on settings). The most important messages cover: tyre management, pit strategy, tactics (undercut/dirty air/defend), weather, and Safety Car / flags. The same advice also appears as text on the Dashboard.

### Live track map

Click the 🗺️ **Map** button in the top-right of the Dashboard to open the live track map in a separate window:
- All cars shown in real time
- Your own car highlighted in yellow
- Tyre compound, gap data, yellow zones marked
- A pulsing yellow banner on top during SC/VSC

---

## 6. Troubleshooting

### "Not connecting" / The Dashboard is empty

1. **UDP telemetry is off in F1 25** → check the game settings (see [section 4](#4-configuring-f1-25))
2. **Wrong IP in F1 25** → if you play on the same PC, the UDP IP should be `127.0.0.1`
3. **Firewall blocks port 20777** → Windows Defender Firewall → Allowed apps → allow F1 Race Engineer
4. **The app didn't finish loading** → close and reopen, wait ~10 seconds after the splash

### The engineer says nothing

1. **Are you in a race session?** The engineer only speaks during a race (silent in qualifying/practice)
2. **Is the volume on?** Check it in Race settings
3. **Windows sound** → make sure the app isn't muted (taskbar → Volume Mixer)
4. **First few laps** → the app needs a few laps to gather enough data for advice

### "Trial expired" / "Invalid license"

- If the 14-day trial expired → enter a license key ([section 3](#3-entering-a-license-key))
- If you lost your key → email f1zeropointracing@gmail.com

### Updates (automatic)

F1 Race Engineer **updates automatically** — no manual download needed. When a new version is released:

1. After launch, an **update banner** appears in the main menu: *"🔄 New version available… ⬇ downloading %… ✅ ready"*
2. The banner also shows **what's new** in this version.
3. Click **"Restart now"** → it installs and restarts. Or **"Later"** → it installs on the next close.

> Your **settings and license key are preserved** after updating — nothing needs to be re-entered. (They live in your user folder, `%APPDATA%\F1RaceEngineer\`, which updates don't touch.)

The latest version can also be downloaded manually (e.g. for a new machine):
**https://github.com/ZeroPointRace/F1-Race-engineer-releases/releases/latest**

### Other problems

If the above didn't help, email support and include:
- What the app did exactly (what you saw, what you heard)
- Which F1 25 version you use (base or 2026 DLC)
- Windows version (Win10 / Win11)

📧 **f1zeropointracing@gmail.com** · 💬 **Discord:** https://discord.gg/fbRscvmJtV

---

## 7. Security and privacy

### Verifying the installer (SHA256)

For every release we publish the installer's **SHA256 checksum** (on the
[releases page](https://github.com/ZeroPointRace/F1-Race-engineer-releases/releases/latest)).
This lets you confirm the downloaded file is **intact and unmodified**:

1. Download the installer
2. Open a PowerShell window and run:
   ```powershell
   Get-FileHash "F1-Race-Engineer-Setup-x.y.z.exe"
   ```
3. Compare the printed value with the one on the releases page — if they **match**, the file is authentic and was not tampered with during download.

### "Unknown publisher" warning

The installer is not currently (paid) **code-signed**, so Windows SmartScreen may show
an "unknown publisher" warning on first run. **The file is safe** — click
**"More info" → "Run anyway"**. You can verify authenticity at any time with the
SHA256 check above.

### What data we handle

The app handles **as little data as possible**, and **never** sends your race data anywhere:

| Data | Purpose | Note |
|---|---|---|
| **Email address** | To deliver your license key | You provide it when requesting a key |
| **Hardware ID (HWID)** | To bind the license to your PC | A **one-way hash** of your CPU/motherboard/disk IDs — not reversible, and it prevents one key from being shared |

> 🔒 **Your race telemetry stays local** — lap times, tyre data and positions
> **never** leave your machine. During license validation the app sends **only** the
> two items above to the server, to verify your key is valid.

Data deletion requests or questions: **f1zeropointracing@gmail.com**

---

*F1 Race Engineer © 2026 ZeroPoint Racing — All rights reserved*
