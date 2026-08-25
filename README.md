<div align="center">

# ⚔️ Pojav Tier Tagger

**See PvP tiers right above every player's head — built for PojavLauncher.**

<img src="https://img.shields.io/badge/Minecraft-1.21.11-62B47A?style=for-the-badge&logo=minecraft&logoColor=white" alt="Minecraft"/>
<img src="https://img.shields.io/badge/Fabric-Loader%200.19.3-DBB69B?style=for-the-badge&logo=fabric&logoColor=black" alt="Fabric"/>
<img src="https://img.shields.io/badge/PojavLauncher-Android-4CAF50?style=for-the-badge&logo=android&logoColor=white" alt="PojavLauncher"/>
<br/>
<img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="License"/>
<img src="https://img.shields.io/github/v/release/OG-BlazeNYX/Pojav-Wiki?style=for-the-badge&color=orange" alt="Release"/>
<img src="https://img.shields.io/github/actions/workflow/status/OG-BlazeNYX/Pojav-Wiki/build.yml?style=for-the-badge&label=Build" alt="Build Status"/>

<br/>

<img src="https://img.shields.io/github/downloads/OG-BlazeNYX/Pojav-Wiki/total?style=flat-square&logo=github" alt="Downloads"/>
<img src="https://img.shields.io/github/stars/OG-BlazeNYX/Pojav-Wiki?style=flat-square&logo=github" alt="Stars"/>
<img src="https://img.shields.io/modrinth/dt/YOUR_MODRINTH_SLUG?style=flat-square&logo=modrinth&label=Modrinth%20downloads&color=1bd96a" alt="Modrinth Downloads"/>

</div>

---

## 📖 What is this?

**Pojav Tier Tagger** is a lightweight Fabric client mod that fetches PvP tier
rankings and displays them as colored badges next to player names — in the
**nametag**, the **tab list**, and **chat**. Built and tuned specifically for
Android devices running Minecraft through **PojavLauncher**.

<div align="center">
<img src="https://img.shields.io/badge/⚡-Lightweight-yellow?style=flat-square"/>
<img src="https://img.shields.io/badge/🎨-Custom%20Tier%20Colors-purple?style=flat-square"/>
<img src="https://img.shields.io/badge/📱-Pojav%20Optimized-brightgreen?style=flat-square"/>
<img src="https://img.shields.io/badge/🧩-Fabric%20API-lightgrey?style=flat-square"/>
</div>

---

## ✨ Features

| | Feature | Description |
|---|---|---|
| 🏷️ | **Live Tier Badges** | Auto-fetched rankings shown beside names in nametag, tab, and chat |
| 🎮 | **Per-Gamemode Icons** | Sword, Mace, SMP, Pot, Vanilla, NethOP, UHC, Axe, Cart, and Diamond SMP all get their own icon |
| 🌈 | **Custom Tier Colors** | HT1 → LT5 each get their own configurable color |
| 🔀 | **Dual Tier Display** | Show **two** tiers at once — one on the left, one on the right — with simple arrow buttons to flip sides |
| 🧍 | **Live Mannequin Preview** | The config screen shows a preview skin that updates in real time as you change settings |
| 🔁 | **Auto-Refresh** | Rankings refresh automatically on a configurable interval |
| ⌨️ | **Keybind + Commands** | Cycle gamemodes with a hotkey, or use `/pojavtier` |
| 🖥️ | **Mod Menu Integration** | Full in-game config screen, no config file editing needed |

---

## 📸 Preview

<div align="center">

```
┌─────────────────────────────────────┐
│   ⚔ HT2  |  Notch  |  LT3 🪓         │
│   ↑ left tier   ↑ name   ↑ right    │
└─────────────────────────────────────┘
```

*Tier badges rendered directly in the nametag, tab list, and chat.*

</div>

---

## 📥 Installation

<div align="center">

<img src="https://img.shields.io/badge/1-Install%20PojavLauncher-4CAF50?style=for-the-badge&logo=android&logoColor=white"/>
<img src="https://img.shields.io/badge/2-Install%20Fabric%20Loader-DBB69B?style=for-the-badge&logo=fabric&logoColor=black"/>
<img src="https://img.shields.io/badge/3-Drop%20the%20.jar%20in%20mods-blue?style=for-the-badge&logo=files&logoColor=white"/>

</div>

1. Set up **[PojavLauncher](https://pojavlauncher.app/)** on your Android device.
2. Install **Fabric Loader** for Minecraft `1.21.11`.
3. Download the latest `pojavtiertagger-*.jar` from the [**Releases**](../../releases) tab.
4. Place it in:
   ```
   .minecraft/mods/
   ```
5. Launch the game — the mod loads automatically. ✅

---

## 🛠️ Configuration

Open the in-game config screen via:

- **Mod Menu** → Pojav Tier Tagger → ⚙️ Config
- or run `/pojavtier config`

<div align="center">
<img src="https://img.shields.io/badge/🔧-Fully%20In--Game%20Configurable-informational?style=for-the-badge"/>
</div>

| Setting | What it does |
|---|---|
| **Enabled** | Master on/off switch |
| **Show Icons** | Toggle gamemode icons next to tier text |
| **Show in Nametag / Tab / Chat** | Control where badges appear |
| **Gamemode** | Which gamemode's tier is your primary badge |
| **Highest Mode** | `Never` / `If none` / `Always` fall back to your overall best tier |
| **Second Tier** | Enable a second badge, pick its gamemode |
| **← / → Arrows** | Choose which side the second tier badge renders on |
| **Refresh Interval** | How often rankings auto-refresh |

---

## ⌨️ Commands

| Command | Description |
|---|---|
| `/pojavtier` | Toggle the mod on/off |
| `/pojavtier config` | Open the config screen |
| `/pojavtier refresh` | Force-refresh rankings |
| `/pojavtier gamemode <mode>` | Set your primary gamemode |
| `/pojavtier player <name>` | Look up a player's tier info |

---

## 🧩 Dependencies

<div align="center">

| Mod | Required |
|---|:---:|
| [Fabric API](https://modrinth.com/mod/fabric-api) | ✅ |
| [Fabric Loader](https://fabricmc.net/) `0.19.3+` | ✅ |
| [Mod Menu](https://modrinth.com/mod/modmenu) | Optional (for in-game config UI) |

</div>

---

## 🏗️ Building from source

```bash
git clone https://github.com/OG-BlazeNYX/Pojav-Wiki.git
cd Pojav-Wiki
./gradlew build
```

The compiled jar will be in `build/libs/`.

<div align="center">
<img src="https://img.shields.io/badge/Built%20with-Gradle-02303A?style=flat-square&logo=gradle&logoColor=white"/>
<img src="https://img.shields.io/badge/Loom-Fabric-DBB69B?style=flat-square&logo=fabric&logoColor=black"/>
<img src="https://img.shields.io/badge/Java-21-ED8B00?style=flat-square&logo=openjdk&logoColor=white"/>
</div>

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to
discuss what you'd like to change.

<div align="center">
<img src="https://img.shields.io/github/issues/OG-BlazeNYX/Pojav-Wiki?style=flat-square"/>
<img src="https://img.shields.io/github/issues-pr/OG-BlazeNYX/Pojav-Wiki?style=flat-square"/>
<img src="https://img.shields.io/github/last-commit/OG-BlazeNYX/Pojav-Wiki?style=flat-square"/>
</div>

---

## 📜 License

This project is licensed under the **MIT License** — see [`LICENSE`](LICENSE) for details.

---

<div align="center">

Made with ❤️ for the Pojav community

<img src="https://img.shields.io/badge/Minecraft-Java%20Edition-brightgreen?style=flat-square&logo=minecraft"/>
<img src="https://img.shields.io/badge/Platform-Android%20%7C%20PojavLauncher-4CAF50?style=flat-square&logo=android"/>

</div>
