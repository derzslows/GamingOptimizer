<div align="center">

# 🎮 Gaming Optimizer

[![Version](https://img.shields.io/badge/version-4.1.0-blue.svg)](https://github.com/derzslows/GamingOptimizer/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011%20(x64)-0078D6.svg?logo=windows)](#-system-requirements)
[![.NET](https://img.shields.io/badge/.NET%208%20%C2%B7%20WinUI%203-512BD4.svg?logo=dotnet)](#)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Languages](https://img.shields.io/badge/i18n-English%20%7C%20Espa%C3%B1ol-orange.svg)](#)

**A powerful, modern and fully‑reversible Windows optimizer for gaming, performance, latency and privacy.**

**English** · [Español](README.es.md)

</div>

> **Guiding principle:** *everything you turn off can be turned back on.* Every change captures its previous state and is reversible — even after a reboot — backed by a persistent journal and an optional Windows restore point before batches.

<div align="center">

![Dashboard](https://github.com/user-attachments/assets/474d4e81-0031-4a40-8e52-e4c9daf4369e)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Screenshots](#-screenshots)
- [Installation](#-installation)
- [System Requirements](#-system-requirements)
- [What's New in 4.1.0](#-whats-new-in-410)
- [Reversibility & Safety](#-reversibility--safety)
- [Disclaimer](#-disclaimer)
- [License](#-license)
- [Author](#-author)

---

## 📝 Overview

**Gaming Optimizer** helps gamers and power users get the most out of Windows. It combines **~170 reversible optimizations**, a **real benchmark** to measure the before/after, a one‑click **Game session** boost, **portable profiles** to share your whole setup, **diagnostics**, **driver management**, **real‑time monitoring** and a full **app manager** — in a single modern interface, in **English and Spanish**.

Unlike one‑shot "tweak scripts", every optimization here is applied through a reversible engine: you can experiment with confidence and roll back any change, individually or all at once.

This project was born, above all, to help friends with no technical background in two situations: **optimizing their Windows installation** without fear of breaking anything, and **getting a PC back up and running after a clean install** — apps installed and settings applied — from a single `.goprofile`.

---

## ✨ Features

### 🎛️ Optimizations — ~170 reversible tweaks
Curated, documented tweaks across **15 categories**: Gaming, CPU, GPU, Memory, Storage, Network, Power, Latency/timers, Input, Appearance/DWM, Privacy/Telemetry, Services, Startup and System. Search and filter, **Easy / Advanced** modes, *Apply recommended* and *Restore all*. No snake‑oil — only real, source‑backed changes.

### 📈 Performance — measure, don't guess *(new in 4.1)*
- **Gaming health score (0–100)**, aware of your hardware: refresh rate vs your monitor's real maximum, power plan, XMP/EXPO, Game DVR, optimization drift, restore points and more. Checks that don't apply to your PC are excluded — nothing penalizes you unfairly. Every pending item has a one‑click **Fix**.
- **Real benchmark (before / after)**: CPU (single & multi‑core), RAM, disk (honest, uncached read) and system latency jitter in ~25 seconds. Run it before and after optimizing and see the actual per‑metric gain. Numbers are comparable on your own PC — no made‑up scores.

### ⚡ Game session — one‑click boost *(new in 4.1)*
A **temporary, fully reversible boost** while you play: maximum power plan, Windows Update / BITS / Delivery Optimization paused, 1 ms system timer. Ending the session restores everything exactly as it was; if you close the app or reboot mid‑session, the dashboard reminds you it's still active — nothing stays half‑done.

### 💾 Portable profiles (.goprofile) *(new)*
Export your whole setup to one small file and share it or restore it after reinstalling Windows: **optimizations (pick categories à la carte), app preferences, and even your installed apps**. Importing shows a full preview first — what applies, what doesn't fit that hardware (NVIDIA‑only tweaks skip cleanly on AMD), what needs confirmation — and the receiver chooses which categories to apply. **Safe by design**: the file only carries tweak IDs, never commands. Double‑click a `.goprofile` and the app opens straight into the preview.

### 📊 Dashboard
Real‑time overview: gaming health score, live network graph (60 s window, active adapter, session peaks), hardware names and models, all drives with usage, CPU/GPU/RAM details, cache and XMP info, Windows activation, and a **Change safety** card showing your latest restore point and journaled changes.

### 🔎 Global search *(new in 4.1)*
A search box in the sidebar that instantly finds any optimization, catalog app or page — and takes you straight there, already filtered.

### 🧰 Tools
- **🆔 Hardware Identification** — every unique ID of your machine in one place: BIOS/SMBIOS, motherboard, CPU (ProcessorID, microcode, cache), GPUs, RAM modules, disks (serial / unique ID / GUID), volumes, partitions, monitors (EDID + SHA‑256), network MAC/GUID, Bluetooth, audio, USB controllers, TPM, Secure Boot, Windows Product ID, Machine GUID & SID — with one‑click **Copy report**.
- **🧩 Drivers** — a complete driver detector, inspector and manager: device drivers, kernel/services and loaded kernel modules, with signature and third‑party info, **anomaly detection** and uninstall of third‑party packages.
- **🖥️ Display** — real monitor model, **HDR** toggle, native resolution, scaling, refresh rate (with "use maximum" warning), rotation and primary‑display switching, read straight from each monitor's EDID.
- **⚡ Power plans & GPU** — reveal/manage power plans (incl. Ultimate Performance) and GPU/driver utilities.
- **🌐 Network** — real‑time traffic monitor, a **per‑process connection inspector**, and a gaming troubleshooting panel: layered connectivity check, packet‑loss/latency/jitter quality test, traceroute and MTU discovery.
- **🚀 Startup** — manage what launches with Windows.
- **📜 Change history** — review everything you've applied and revert entries individually or all at once; the dashboard warns if Windows Update or another tool silently undoes your optimizations (**drift detection**).

### 🧹 Maintenance
- **📦 Apps & Debloat** — a full app manager in three tabs:
  - **Install**: ~250 curated apps via `winget` (browsers, gaming, emulators, dev, monitoring, security…) with search, categories, **batch install** and a per‑app **details card** (ⓘ): real system info for installed apps, full description/publisher/license for the rest.
  - **Update**: every app on your PC with a pending update — one by one or **all at once with live progress**; stubborn installers get a "Retry in window" option.
  - **Remove**: uninstall preinstalled UWP bloatware, and uninstall catalog apps (always with confirmation).
- **🧽 Cleanup** — reclaim disk space safely, including **shader caches** (DirectX, NVIDIA, AMD, Intel) to fix post‑driver‑update stutter.

### 🔒 Security ↔ Performance module *(Advanced, opt‑in)*
Optionally toggle **VBS**, **Memory Integrity (HVCI)**, **Spectre/Meltdown mitigations**, **Credential Guard** and the **hypervisor** — each with clear warnings and full reversibility. Hidden in Easy mode and gated behind explicit confirmation.

### Also
♻️ Fully reversible engine · 🖼️ Modern, **responsive UI** (reflows to ultrawide/high‑DPI) · 🌍 English & Spanish · 🔄 Automatic updates.

---

## 📸 Screenshots

| Dashboard | Optimizations |
|---|---|
| ![Dashboard](https://github.com/user-attachments/assets/474d4e81-0031-4a40-8e52-e4c9daf4369e) | ![Optimizations](https://github.com/user-attachments/assets/db89651e-5563-49b1-9aeb-7388f95f3e1b) |
| **Network Tools** | **Apps Installer** |
| ![Network Tools](https://github.com/user-attachments/assets/4f1969de-54ba-4230-9b52-7365fb29059c) | ![Apps Installer](https://github.com/user-attachments/assets/26254cb3-97bc-41de-b4dd-1fbac9d14e79) |

---

## 📥 Installation

1. Download **`GamingOptimizer-x.y.z.msi`** from the [latest release](https://github.com/derzslows/GamingOptimizer/releases/latest).
2. Run the installer (you'll be prompted to confirm administrator rights).
3. If you already have an older version, it **updates automatically**.

The app is self‑contained — the .NET runtime is bundled, nothing else to install. The installer also associates **`.goprofile`** files, so shared profiles open with a double‑click.

---

## ⚙️ System Requirements

| | |
|---|---|
| **OS** | Windows 10 or Windows 11 (64‑bit) |
| **Privileges** | Administrator (the app runs elevated) |
| **Runtime** | None — bundled in the installer |

---

## 🚀 What's New in 4.1.0

- 📈 **Performance page**: hardware‑aware gaming health score (0–100) with one‑click fixes + a **real before/after benchmark** (CPU, RAM, uncached disk, latency jitter).
- ⚡ **Game session**: one‑click temporary boost (max power plan, updates paused, 1 ms timer), fully journaled and reversible.
- 🔎 **Global search** across optimizations, apps and pages.
- 📦 **Apps & Debloat, rebuilt**: tabs, ~250 curated apps, batch install, per‑app details cards, a full **Update** tab with live progress and "Retry in window", and uninstall with confirmation.
- 💾 **Profiles**: your installed apps travel inside the `.goprofile`, categories are selectable on both export and import (à la carte), and profiles open with a double‑click.
- 🧹 Shader‑cache cleanup extended to AMD (OpenGL/Vulkan) and Intel.

<details>
<summary>4.0.x</summary>

- **4.0.3** — Display page fix: the first monitor was missing on multi‑monitor setups.
- **4.0.2** — **Portable profiles (.goprofile)**: export/import your optimization setup safely across different hardware; richer dashboard (live network graph, change‑safety card).
- **4.0.0** — Complete **Fluent / Windows 11 redesign** (Mica, light/dark theme); network gaming troubleshooting panel; display refresh‑rate warning + HDR toggle with timed confirmation; **Change history** page and **drift detection**; 8 new optimizations; honest security status; self‑contained installer.

</details>

<details>
<summary>3.0.0 and earlier</summary>

- **3.0.0** — Hardware Identification and Drivers manager; optimization catalog nearly doubled (86 → 166); advanced Security ↔ Performance module; fully responsive UI.
- **2.0.0** — Far more complete Dashboard; network traffic monitor and per‑process connection inspector; redesigned Apps & Debloat, Cleanup and Startup.

</details>

---

## ♻️ Reversibility & Safety

Optimizations run through a reversible engine: `ITweak → ISystemChange → persistent journal`. Each change records the previous value before applying, so it can be reverted later — even across reboots. Registry changes restore the exact prior value; command/policy changes restore Windows defaults. Batches can create a **Windows restore point** first, and importing a profile always does. There is **no registry "cleaner"**, and the optimization catalog leaves Microsoft Defender, BitLocker and Windows Update services alone — the **Game session** pauses Windows Update only while you play, journaled and restored when it ends.

---

## ⚠️ Disclaimer

This tool changes Windows system settings. Although every change is reversible, some optimizations — especially those in the **Security ↔ Performance** module — reduce protections or affect stability and are intended for personal, trusted PCs. Use at your own risk, and create a restore point before applying large batches.

---

## 📄 License

Released under the **MIT License** — see [LICENSE](LICENSE).

---

## 👤 Author

**derzslows** — [@derzslows](https://github.com/derzslows)

<div align="center">

⭐ *If this project is useful to you, consider leaving a star!*

Made with ❤️ for gamers and Windows power users.

</div>
