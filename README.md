
# **ZCleaner 🚀**

A fast, lightweight, privacy-respecting cleaner and system monitor for macOS.

Built with **Tauri (Rust + React)** for performance and a beautiful UI.

## **✨ Features (Planned)**
- **Smart Cleaning**
  - Remove leftover caches, logs, and app junk (safe by default).
  - Recipes for popular tools: Xcode, Docker Desktop, OrbStack, VS Code, package managers, etc.
  - One-click preview of reclaimable space before deleting.
- **System Monitor (Menu Bar Widget)**
  - CPU load, memory usage, disk space, and network activity.
  - Optional extras: CPU temperature & fan speed (outside App Store only).
  - Always-on-top tray window with a compact dashboard view.
- **Developer-Friendly Tools**
  - Identify heavy dev caches (npm, pnpm, yarn, pip, cargo, gradle, Xcode DerivedData, etc.).
  - Clean simulator/device leftovers.
- **Safety First**
  - Default to **moving items to Trash** (reversible).
  - Clearly show what’s safe vs. advanced removal.
  - Respect user privacy — no tracking, no phoning home.

## **🛠 Tech Stack**
- **UI:** React + Tauri (Webview)
- **Backend:** Rust (fast filesystem scanning, system stats)
- **Bridge:** Tauri commands for scanning, trash/delete, stats collection
- **Packaging:** macOS notarization & Developer ID distribution

## **📦 Roadmap**
- File/folder scanner (show top space hogs)
- Trash/Delete actions
- Configurable “recipes” for common apps
- Menu bar system monitor
- Autostart at login
- Dark/light mode support
- Signed and notarized macOS release

## **⚠️ Notes**
- CPU temperature and fan speed are only possible with private macOS APIs → these features won’t be available in a Mac App Store build.
- ZCleaner will focus on **transparency and control**, not “magic optimizations”.

## **🤝 Contributing**

Ideas, bug reports, and feature suggestions are welcome!

Please open an issue or pull request to discuss changes.
