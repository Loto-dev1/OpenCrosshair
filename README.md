<div align="center">

# 🎯 OpenCrosshair

**The lightweight, zero-latency crosshairs overlay built natively for Linux gaming.**

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=flat-square)](https://www.gnu.org/licenses/gpl-3.0)
[![Linux Support](https://img.shields.io/badge/Linux-Wayland%20%7C%20X11-informational?style=flat-square&logo=linux&logoColor=white)](https://kernel.org)
[![Built with Tauri](https://img.shields.io/badge/Built%20with-Tauri%20v2-FFC131?style=flat-square&logo=tauri&logoColor=black)](https://v2.tauri.app)
[![Rust Core](https://img.shields.io/badge/Core-Rust-000000?style=flat-square&logo=rust&logoColor=white)](https://www.rust-lang.org)

[Features](#-features) • [Compositor Support](#-compositor-compatibility) • [Quick Start](#-quick-start) • [Privacy](#-privacy)

</div>

---

## 🚀 Why OpenCrosshair?

Most overlay tools on Linux are either clunky Python scripts, heavy Electron apps that drain system resources, or simply don't support modern Wayland compositors.

**OpenCrosshair** solves this. Built from the ground up in **Rust + Tauri v2**, it runs as a native transparent overlay with **zero performance loss**, full hardware click-through, and instant customization.

---

## ✨ Features

* ⚡ **Ultra-Low Resource Footprint:** Uses less than 15 MB RAM and 0% idle CPU usage.
* 🐧 **Wayland & X11 Native:** Native integration for layer-shell protocols and X11 window overlays.
* 🖱️ **Hardware Click-Through:** Mouse clicks pass straight through the crosshair to your game with zero lag.
* 🎨 **Real-Time Editor:** Fine-tune dot size, gap, line thickness, outline, opacity, and custom hex colors.
* 🌐 **Anonymous Preset Hub:** Download and share community crosshair presets without signing up.
* 🔒 **Zero Telemetry:** No login, no background analytics, no hidden data tracking.

---

## 🖥️ Compositor Compatibility

| Compositor / Desktop | Protocol | Overlay Status | Click-Through |
| :--- | :--- | :---: | :---: |
| **Hyprland** | Wayland | ✅ Supported | ✅ Hardware |
| **Sway** | Wayland | ✅ Supported | ✅ Hardware |
| **KDE Plasma (6 / 5)** | Wayland / X11 | ✅ Supported | ✅ Hardware |
| **GNOME** | Wayland / X11 | ✅ Supported | ✅ Hardware |
| **Xfce / i3 / bspwm** | X11 | ✅ Supported | ✅ Hardware |

---

## 🛠️ Quick Start

### Prerequisites (Arch / Ubuntu / Fedora)

```bash
# Arch Linux / EndeavourOS
sudo pacman -S --needed base-devel webkit2gtk-4.1 cairo pango

# Ubuntu / Debian / Pop!_OS
sudo apt install build-essential libwebkit2gtk-4.1-dev libgtk-3-dev
