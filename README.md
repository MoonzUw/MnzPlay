MnzPlay

Single-file web gaming and emulation portal (index.html) featuring an interactive catalog, main-menu controller support, a Steam-style friends system, cloud-persisted chat, and Supabase integration.
Features

    Catalog & Navigation: Games, Favorites, and Recent tabs, instant search, and filtering by system (N64, SNES, Web / JS).

    3D Physical Media: Front-and-back flip view with game details and support for customizing front and back cover art locally in the browser.

    In-Browser Emulation: Runs via EmulatorJS (with local ROM loading through the ROM button) alongside shortcuts for web links/ports.

    Controller (Gamepad API): D-Pad/analog navigation, button shortcuts, configurable deadzone, and status indicators in the top bar.

    Friends & Cloud Chat: Friends list grouped by status (In-Game, Online, Offline), current game presence, and messages saved in Supabase with local caching in localStorage.

Architecture & Backend

    Frontend: Self-contained index.html (HTML, CSS, and JavaScript).

    Supabase: Authentication, perfis profiles table, and mensagens message persistence.

Hosting

    GitHub Pages: Published from the main branch at the repository root (/ (root)).

    Cloudflare Pages: Static mirror/hosting connected to the repository for redundancy.

ROM Notice

ROMs are not distributed with the repository; use the ROM button inside the player to load your own files (.z64, .n64, .v64, .sfc, .smc) directly in the browser.
