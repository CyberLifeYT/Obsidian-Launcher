# Obsidian Launcher

**Obsidian Launcher** is a custom, Minecraft: Java Edition launcher built with WPF.  
It downloads official Mojang version metadata and assets directly, supports local (offline) accounts, and lets you install **Fabric** and **Forge** mod loaders with a single click – plus an integrated **Mod Browser** to search and install community mods.

![Obsidian Launcher Screenshot](screenshots/Launcher.png)

---

## ✨ Features

- 🔹 **Fully Offline** – No Microsoft account required; use local usernames.
- 🔹 **Version Manager** – Browse and download any Minecraft release or snapshot from Mojang’s manifest.
- 🔹 **Mod Loader Integration**  
  - Install **Fabric** – lightweight, modern modding.  
  - Install **Forge** – the classic, widely‑used mod platform.
- 🌐 **Built‑in Mod Browser** *(new in v1.1.2)*  
  Search, browse, and install mods from **CurseForge** and **Modrinth** directly inside the launcher.  
  Filter by mod loader, view descriptions and download counts, and manage installed mods.
- 🧠 **Smart Java Detection** – Automatically finds Java 17/21 from common paths, system `PATH`, and the Windows registry.
- 🛠️ **Custom JVM Settings** – Configure memory allocation, additional JVM arguments, and Java executable path.
- 📦 **Download Progress** – Real‑time library and asset download tracking with progress bars.
- 🚀 **One‑Click Launch** – Select a version, add an account, and hit **PLAY**.
- 🔄 **Built‑in Updater** – Checks GitHub releases and can update itself with a single click.

---

## 🖥️ Requirements

- Windows 10 / 11 (64‑bit)
- **Java Runtime 21 or later** (Java 17 may work for older versions; see [Troubleshooting](#troubleshooting))
- .NET Framework 4.8 (the launcher is self‑contained, no extra installation required)

---

## 🚀 Getting Started

### Pre‑built Release (recommended)
1. Go to the [Releases](https://github.com/CyberLifeYT/Obsidian-Launcher/releases) page.
2. Download the latest `ObsidianLauncher.exe`.
3. Run it – no installation needed.

### First Launch
- The launcher will try to auto‑detect a Java installation. If it fails, go to **Settings → Java** and browse to your `javaw.exe` (e.g. `C:\Program Files\Eclipse Adoptium\jdk-21.0.5+11\bin\javaw.exe`).
- In the **Versions** tab, select a Minecraft version and download it.
- Add a local account in the **Account** tab (any username ≥3 characters).
- (Optional) Install Fabric or Forge in the **Mod Loader** tab, then browse and install mods in the **Browse Mods** sub‑tab.
- Go to the **Play** tab and press **PLAY**.

---

## ❗ Troubleshooting

### “Game failed to start (exit code 1) – UnsupportedClassVersionError”
This means you’re using an older Java version while Minecraft requires **Java 21**.  
**Fix:** Download and install **Java 21** from [Adoptium](https://adoptium.net/), then point the launcher to its `javaw.exe` in **Settings → Java**.

### “The system cannot find the file specified”
The launcher cannot locate a Java executable.  
**Fix:** Make sure Java is installed and the path is set correctly in **Settings → Java**. If you just installed Java, restart the launcher so it can re‑detect.

### Launcher minimises then reappears without the game starting
This usually means the game crashed instantly. The launcher now shows the exact error (requires v1.1.1 or later). If you don’t see the error, update to the latest version – it includes better crash reporting.

### “The calling thread cannot access this object” (v1.1.1+)
This crash has been **fixed** in v1.1.1 and later. Update to the latest release to solve it.

---

## 🔄 Updating

The launcher checks for updates automatically on startup.  
You can also manually check under **Settings → Check for Updates**.

---

## 📃 Changelog

### v1.1.2 (current)
- **Mod Browser** – search and install mods from CurseForge and Modrinth directly.
- All ComboBox dropdowns now show black text for better readability.
- Various UI polish and stability improvements.

### v1.1.1
- Fixed cross‑thread crash when launching the game.
- Vastly improved Java auto‑detection (system PATH, registry, common folders).
- Detailed error messages when the game fails to start (Java version, missing files, etc.).

### v1.1.0
- Fabric installer integration.
- Forge installer integration.
- Auto‑updater via GitHub releases.
- Mod loader badge in the sidebar.

### v1.0.0
- Initial release with full vanilla version downloading, offline accounts, JVM settings.

---

## 📜 License
MIT – feel free to use, modify, and share.

---

_Obsidian Launcher is not affiliated with Mojang or Microsoft. “Minecraft” is a trademark of Mojang AB._
