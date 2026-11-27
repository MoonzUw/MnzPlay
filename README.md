# MnzPlay

A single-file web gaming and emulation portal (`index.html`) built with vanilla HTML, CSS, and JavaScript, featuring an interactive catalog, 3D physical media cards, main-menu controller support, a Steam-style friends list, chat, and optional Supabase cloud integration.

---

## ✨ Features

* **Catalog & Navigation:** *Games*, *Favorites*, *Recent*, *Friends*, *Achievements*, and *Settings* tabs, with instant search and system filtering (`N64`, `SNES`, `WEB`).
* **3D Physical Media:** Front-and-back card flip view showing game details, launch actions, and custom front/back cover art saved locally in the browser.
* **In-Browser Emulation:** Powered by **EmulatorJS** (`n64` and `snes`) with local ROM loading directly inside the player, plus links/shortcuts for external `WEB` titles.
* **Controller & Input Support:** Gamepad API support with D-pad/analog navigation, adjustable deadzone, button shortcuts, and keyboard controls.
* **Friends & Chat:** Friends list grouped by status (*In-Game*, *Online*, *Offline*), live/current game display, profile photo & nickname customization, and cloud-synced chat when signed in.
* **Language Detection:** Automatic initial locale detection with support for `pt-BR`, `en`, and `es`.

---

## 🏗️ Architecture & Backend

* **Frontend:** Self-contained `index.html` (HTML, CSS, and JavaScript with no build step required).
* **Local Storage:** Favorites, recents, settings, custom covers/backs, profile photo, and local session state persist in `localStorage` (loaded ROMs stay in browser memory for the active session only).
* **Cloud (Supabase):** Authentication and sync backed by the `perfis` and `mensagens` tables, with seamless local/guest fallback when unconfigured or offline.

---

## 🚀 Hosting

* **GitHub Pages:** Published from the main branch at the repository root (`/`).
* **Cloudflare Pages:** Connected static deployment mirror for redundancy.

---

## ⚠️ ROM Notice

ROMs are **not** included in this repository. Use the **ROM** button inside the player to load your own compatible ROM files (`.z64`, `.n64`, `.v64`, `.sfc`, `.smc`) directly in the browser.
