
# **ZCleaner Roadmap 🗺️**

A staged plan for building **ZCleaner**, the macOS cleaner + system monitor.

---

## **🎯 v0.1 — Proof of Concept (Local Only)**
- CLI prototype in Rust to scan common folders (Caches, Logs, Downloads).
- Display top N largest files/folders.
- Basic React UI in Tauri (file list, size display).
- Button to move selected items to Trash.
- Simulate-only mode (no deletions).

---

## **🚀 v0.2 — Core Cleaner**
- Configurable **recipes.json** for known apps (Xcode, Docker, VS Code, package managers).
- Add “Move to Trash” vs “Delete Permanently”.
- Basic safety checks (block critical system folders).
- Disk usage overview card (per volume).
- Export report (Markdown/JSON of what was cleaned).

---

## **🖥️ v0.3 — Menu Bar Monitor**
- Add system tray/menu bar icon.
- Popover window showing:
  - CPU load %
  - Memory usage
  - Disk usage
  - Network I/O rates
- Background Rust task to poll stats (every 1–2s).
- Option to auto-start at login.

---

## **🌗 v0.4 — UI & UX Polish**
- Dark/light mode support.
- Progress indicators during scan/clean.
- “Open in Finder” option per item.
- Settings screen (exclude folders, auto-clean rules).
- Multilingual support (starting with English).

---

## **🧑‍💻 v0.5 — Developer Tools**
- Deeper scanning of dev caches:
  - ~/.npm, ~/.pnpm-store, ~/.yarn, ~/.cache/pip, ~/.cargo, ~/.gradle
- Xcode simulator/device cleanup.
- Show age of cache files (e.g. >30 days old).
- Quick action: “Clean all dev caches”.

---

## **🔒 v0.6 — Stability & Safety**
- Signed + notarized macOS builds (Developer ID).
- First-run onboarding (explain permissions, Full Disk Access if needed).
- Logging + error reporting (local only, no telemetry).
- Configurable exclusions.

---

## **🌟 v1.0 — Public Release**
- Full-featured cleaner + system monitor.
- Tested on Intel + Apple Silicon Macs (macOS 13+).
- Website + documentation.
- Auto-updater (Tauri updater).
- Distribute via DMG installer.

---

## **🔮 Future Ideas (Post-1.0)**
- Smart scheduling (weekly/monthly auto-clean with notifications).
- Plugin system for community-contributed cleaning recipes.
- Optional cloud sync of settings (privacy-preserving).
- Integration with package managers (e.g. prune old Homebrew versions).
- Custom “big file hunter” tool (find >1 GB files anywhere).
- iStat-like extended metrics (if non-App-Store distribution).
