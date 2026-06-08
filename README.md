<div align="center">

# 🎮 Gaming Optimizer

[![Version](https://img.shields.io/badge/version-3.0.0-blue.svg)](https://github.com/derzslows/GamingOptimizer/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011%20(x64)-0078D6.svg?logo=windows)](#-system-requirements)
[![.NET](https://img.shields.io/badge/.NET%208%20%C2%B7%20WinUI%203-512BD4.svg?logo=dotnet)](#-build-from-source)
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
- [What's New in 3.0.0](#-whats-new-in-300)
- [Build from Source](#-build-from-source)
- [Reversibility & Safety](#-reversibility--safety)
- [Disclaimer](#-disclaimer)
- [License](#-license)
- [Author](#-author)

---

## 📝 Overview

**Gaming Optimizer** helps gamers and power users get the most out of Windows. It combines **diagnostics**, **driver management**, an extensive catalog of **reversible optimizations**, **real‑time monitoring** and **cleanup tools** in a single modern, fully responsive interface — in **English and Spanish**.

Unlike one‑shot "tweak scripts", every optimization here is applied through a reversible engine: you can experiment with confidence and roll back any change, individually or all at once.

---

## ✨ Features

### 🎛️ Optimizations — 160+ reversible tweaks
Curated, documented tweaks across **15 categories**: Gaming, CPU, GPU, Memory, Storage, Network, Power, Latency/timers, Input, Appearance/DWM, Privacy/Telemetry, Services, Startup and System. Search and filter, **Easy / Advanced** modes, *Apply recommended* and *Restore all*. No snake‑oil — only real, source‑backed changes.

### 📊 Dashboard
Real‑time overview: hardware names and models, all drives with usage, live network throughput, CPU/GPU/RAM details, base clock/cores/sockets, L1/L2/L3 cache, RAM speed/XMP, Windows license/activation, active sessions and process count.

### 🧰 Tools
- **🆔 Hardware Identification** — every unique ID of your machine in one place: BIOS/SMBIOS, motherboard, CPU (ProcessorID, microcode, cache), GPUs, RAM modules, disks (serial / unique ID / GUID), volumes, partitions, monitors (EDID + SHA‑256), network MAC/GUID, Bluetooth, audio, USB controllers, TPM, Secure Boot, Windows Product ID, Machine GUID & SID — with one‑click **Copy report**.
- **🧩 Drivers** — a complete driver detector, inspector and manager: device drivers, kernel/services and loaded kernel modules, with signature and third‑party info, **anomaly detection** and uninstall of third‑party packages.
- **🖥️ Display** — real monitor model, **HDR** support, native resolution, scaling, refresh rate, rotation and primary‑display switching, read straight from each monitor's EDID.
- **⚡ Power plans & GPU** — reveal/manage power plans (incl. Ultimate Performance) and GPU/driver utilities.
- **🌐 Network** — real‑time traffic monitor, a **per‑process connection inspector**, and network tools (DNS, ping, diagnostics).
- **🚀 Startup** — manage what launches with Windows.

### 🧹 Maintenance
- **📦 Apps & Debloat** — install 150+ curated apps via `winget` (browsers, gaming, dev, monitoring, security…) with search and categories; remove preinstalled UWP bloatware.
- **🧽 Cleanup** — reclaim disk space safely.

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

The app is self‑contained — the .NET runtime is bundled, nothing else to install.

---

## ⚙️ System Requirements

| | |
|---|---|
| **OS** | Windows 10 or Windows 11 (64‑bit) |
| **Privileges** | Administrator (the app runs elevated) |
| **Runtime** | None — bundled in the installer |

---

## 🚀 What's New in 3.0.0

- 🆕 Two new tools: **Hardware Identification** and **Drivers** manager.
- ⚡ Optimization catalog nearly doubled (**86 → 166**), plus an advanced **Security ↔ Performance** module.
- 🖼️ **Fully responsive UI** across every page (multi‑column reflow on wide displays).
- 🖥️ **Display fixes** — HDR, native resolution and manufacture year now read correctly from EDID.

<details>
<summary>2.0.0</summary>

- Far more complete Dashboard; more gaming/performance/privacy optimizations.
- Network traffic monitor and per‑process connection inspector.
- Redesigned Apps & Debloat, Cleanup and Startup.

</details>

---

## 🛠️ Build from Source

**Stack:** WinUI 3 / Windows App SDK 1.8 · .NET 8 · `win-x64` (unpackaged) · CommunityToolkit.Mvvm · Microsoft.Extensions.Hosting (DI) · WiX Toolset v3 (MSI).

**Prerequisites:** [.NET 8 SDK](https://dotnet.microsoft.com/download), the *Windows App SDK* workload, and (for the installer) [WiX Toolset v3](https://wixtoolset.org/).

```powershell
# Build (Debug)
dotnet build .\GamingOptimizer.App\GamingOptimizer.App.csproj -c Debug

# Run (prompts UAC — runs elevated)
Start-Process ".\GamingOptimizer.App\bin\Debug\net8.0-windows10.0.19041.0\win-x64\GamingOptimizer.App.exe"

# Tests
dotnet test .\GamingOptimizer.Tests\GamingOptimizer.Tests.csproj
```

For versioning, publishing and building the MSI there is a small GUI tool — **`builder.ps1`** — that bumps the version everywhere, builds the self‑contained app + updater, regenerates the file list and produces the installer (including the build‑time choice for the optional NG Sentinel agent: *never / optional / on by default*).

> ⚠️ To rebuild the `.exe`, **close the running app first** — if it's open, the code compiles but copying the executable fails (`MSB3021/3027`).

### Project structure

| Project | Role |
|---|---|
| `GamingOptimizer.App` | WinUI 3 UI (MVVM Toolkit, MS.Extensions.Hosting DI) |
| `GamingOptimizer.Core` | Contracts/abstractions, enums, `ITweak` / `ISystemChange` |
| `GamingOptimizer.Platform` | Windows implementations: engine, change primitives, tweaks, GPU/network/power… |
| `GamingOptimizer.Update` | Standalone updater (downloads the GitHub release) |
| `GamingOptimizer.Installer` | WiX (MSI) — outside the `.sln` |
| `GamingOptimizer.Tests` | xUnit (engine + journal + catalog) |

---

## ♻️ Reversibility & Safety

Optimizations run through a reversible engine: `ITweak → ISystemChange → persistent journal`. Each change records the previous value before applying, so it can be reverted later — even across reboots. Registry changes restore the exact prior value; command/policy changes restore Windows defaults. Batches can create a **Windows restore point** first. There is **no registry "cleaner"** and Microsoft Defender / BitLocker / Windows Update services are left alone.

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
