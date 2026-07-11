# Changelog — F1 ZeroPoint Race Engineer

User-facing new features and fixes per release. Newest version on top.

> While working, add lines under the **`## [Unreleased]`** section. On release it is
> renamed to the version number and automatically published to the Manual repo.

## [Unreleased]
- (new features for the next release go here)

## v1.0.11 — 2026-07-11
- 🚦 **Govee flag light support:** your Govee smart light shows race flags in real time (green, local yellow for your own sector, blue, red, Safety Car). Pick the light and set per-event colour, brightness and blink in Settings.
- 🌬️ **Wind simulator support:** speed-based wind via Arduino + fans, configurable in Settings (port, speed range, strength).
- 🏁 **Automatic return to the main menu at the end of a race** (previously it stayed on the Race view).
- 🚦 The Govee flag light now **turns off when you exit** the app.
- 🛠️ **Fixed the contact-support buttons** (in the licence warning and on the Licence page): one click sends your log to support.

## v1.0.9 — 2026-06-26
- 🔒 **More reliable, offline-capable licence protection:** licence and trial checks are now based on a cryptographically signed key — it works reliably offline (up to 30 days) and only stops on an actual revocation. One internet connection is needed after updating.
- 🌐 The "internet required" message now appears in every supported language.

## v1.0.8 — 2026-06-21
- 🔑 **More reliable licence/trial:** a temporary internet outage no longer locks you out — the app keeps working offline (the trial for its remaining days, an activated licence for 30 days), and only stops on an actual licence revocation.

## v1.0.7 — 2026-06-20
- 🌐 **PC IP in the main menu at startup:** your PC's IP now shows right away on launch (previously only after opening the Race view).
- 🪟 **Windows 11 compatibility:** licence activation and the trial now work reliably on newer Windows 11 (24H2).

## v1.0.6 — 2026-06-19
- 🛠️ **Report a problem button:** if something isn't working, send your log to support with one click from the main menu — so we can help you faster.

## v1.0.5 — 2026-06-13
- 💬 Discord community button in the main menu.
- 🇬🇧 The English voice race engineer is now complete — every call-out is available in English.
- 🔧 Minor fixes (language page layout).

## v1.0.4 — 2026-06-11
- 🔧 Minor bug fixes.

## v1.0.3 — 2026-06-07
- 🔔 **Update banner:** the app now notifies you as soon as an update is available (not only after download), shows the download progress, and offers "Restart now / Later".
- 📜 **Changelog:** each release's news appears in the update banner and on the Manual page.

## v1.0.2 — 2026-06-07
- 🔄 **Auto-update:** the app detects, downloads and installs new versions on its own — no more manual downloads.
- 🔢 The version number in the bottom-left corner now always shows the **currently installed version**.

## v1.0.1 — 2026-06-07
- 📋 The **"Copy PC IP"** button in the main menu now works (one click to paste into the F1 25 telemetry settings).

## v1.0.0 — 2026-06-07
- 🎉 **First public release.**
- 🔊 **Hungarian voice race engineer** (and more languages), with real-time advice.
- 🗺️ Live track map, telemetry dashboard, strategy and tyre-management suggestions.
- 🏎️ F1 25 + 2026 DLC (24 cars, Overtake/Boost) support.
- 🎮 Steering-wheel button bindings for voice queries (weather, strategy, nearby cars).
