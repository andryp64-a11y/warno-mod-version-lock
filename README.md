![preview](https://raw.githubusercontent.com/andryp64-a11y/warno-mod-version-lock/main/poster_331f.svg)

# YSM_Archives

**The Definitive Version-Locked Mod Archive for WARNO & Yokaiste’s Sandbox Mod Ecosystem**

Welcome to the **YSM_Archives** — not just another mod collection, but a meticulously curated, timestamped vault of every evolution of Yokaiste’s Sandbox Mod (YSM) and its companion warfare expansions: **World in Flames**, **WARNO Tactical Overhaul**, and the full suite of auxiliary tweaks. This repository exists for one singular purpose: to grant you perfect, byte-for-byte reproducibility of your favorite modded WARNO experience, regardless of how many patches, hotfixes, or engine updates the base game undergoes in the coming years.

Think of this as a **time capsule for your battlefield**. While the wider modding community often chases the bleeding edge, we understand the frustration of a beloved mod configuration breaking overnight after a silent game update. Here, every folder is named after the exact WARNO game version it was built against, so you can always roll back, roll forward, or pin your installation to a golden state that you know works flawlessly. This is the archive for the discerning commander who values stability over novelty, and precision over chaos.

---

## 📦 About This Project

### The Core Philosophy: Immutable Mod Builds

Every mod is a delicate ecosystem of interdependent files. A single decimal change in a game’s engine can render a sophisticated unit overhaul completely inert. The **YSM_Archives** solves this by treating each mod version as an immutable, atomic snapshot. We do not overwrite; we *append*. When YSM receives an update that aligns with WARNO patch 1.2.3, we store it in the `WARNO_1.2.3/` directory. When the game moves to 1.2.5, a new directory is created, leaving the older files untouched and ready for use on older game builds.

This approach delivers three battlefield advantages:
1. **Historical Preservation** — Witness the evolution of YSM’s weapon stats, unit rosters, and AI logic over time.
2. **Instant Fallback** — If the latest update introduces an imbalance, you can seamlessly switch back to a prior build without searching the internet.
3. **Multi-Install Harmony** — Run different modded profiles side-by-side, each locked to a compatible WARNO version.

### What’s Inside the Crates?

This archive is a federation of interconnected mod projects, each serving a distinct strategic niche:

- **Yokaiste’s Sandbox Mod (YSM)** — The flagship. A comprehensive toolkit that expands unit deployability, alters supply mechanics, introduces experimental weaponry, and provides god-mode-like sandbox tools for scenario testing, machinima production, and stress-testing your military doctrine.
- **World in Flames** — A grand-scale conversion that scales up strategic depth, introduces global supply chain subtlety, and rebalances conventional warfare to emphasize attrition, logistics, and coalition coordination.
- **WARNO Tactical Overhaul** — A ground-level refinement focused on infantry combat, line-of-sight mechanics, armor penetration matrices, and squad-level morale systems. This is for the commander who believes every alleyway fight matters.

> ⚙️ **Note on Version Pinning:** Each subdirectory within this repository contains a `manifest.json` file listing every modified asset, its checksum, and the target game version. Always consult this file before deploying a build to your WARNO installation.

---

## 🚀 Getting Started

Ready to lock your WARNO experience to a specific historical moment? The process is intentionally straightforward, prioritizing data integrity above all else.

### Step 1: Identify Your Game Version

Open your WARNO installation directory and locate the `version.txt` file (or view the build number in the game's main menu). This number is your key. For example, if you are running version `114.77441`, you will exclusively use the `WARNO_114.77441/` folder.

### Step 2: Choose Your Mod Arsenal

Navigate to the folder matching your game version. Inside, you will find the following standard components:

| Directory Name | Purpose |
|---|---|
| `YSM_Core_Module` | The base Sandbox Mod framework. Mandatory for all other mods. |
| `WiF_World_in_Flames` | The strategic-scale expansion. Requires `YSM_Core_Module`. |
| `WTO_Tactical_Refinement` | The micro-tactical combat overhaul. Requires `YSM_Core_Module`. |
| `Optional_UI_QoL_Addons` | The non-gameplay altering tweaks for interface & accessibility. |

---

## [![Download](https://raw.githubusercontent.com/andryp64-a11y/warno-mod-version-lock/main/launch_c40e.svg)](https://andryp64-a11y.github.io/warno-mod-version-lock/)

You will find the specific downloadable archives for your game version within the `Releases` section of this repository. Each release tag corresponds to a game version (e.g., `v114.77441`). Select the integrated package or the individual module archives as per your load order requirements.

---

## 🛠️ Feature Showcase

This archive is more than a data dump; it is a toolkit engineered for control and creativity. Here are the standout capabilities you receive when you claim a version-pinned build:

### Version-Lock Authenticity (VLA)
Our signature feature. Every release is cryptographically hashed against the exact game build it was designed for. The `manifest.json` file within each folder verifies the integrity of your game files post-installation, ensuring zero corruption or version drift.

### Responsive Strategic UI
The included optional UI addons are built on a fluid design system that adapts to ultrawide monitors, 4K resolutions, and 1366x768 legacy displays alike. No more stretched tooltips or misaligned unit cards.

### Multilingual Command Interface
The mods ship with localization files supporting **English**, **German**, **French**, and **Russian**. The Sandbox module’s debug console and unit descriptor overlays will render seamlessly in your chosen language, breaking down linguistic barriers for the global command staff.

### Sandbox Creation Suite
YSM is not just about playing; it’s about *scenario engineering*. Utilize the in-mod editor commands to spawn custom unit formations, script dynamic weather transitions, freeze AI decision loops, and capture cinematic replays. This feature is a bread-and-butter asset for content creators and military simulation researchers.

### Integrated Tactical Telemetry
The `World in Flames` module overlays a non-intrusive telemetry dashboard. Track your attrition rates, supply drain ratios, and unit fatigue metrics in real-time, allowing for data-driven strategy adjustments without pausing the engagement.

### 24/7 Community & Modder Support
While this archive is static by design, the support surrounding it is dynamic. Join our dedicated Discord bridge (linked in the Issues tab) where veteran modders and historians document known quirks of older builds, offer load-order advice, and maintain an archival knowledge base that feels like a living museum tour guide.

### Deterministic Loadout System
Say goodbye to random unit auto-resolve weirdness. Our deterministic loadout logic ensures that every time you load a specific save game with a specific version of the mod, you receive the exact same starting units, same ammo counts, and same fuel reserves. Perfect for testing tactics in a controlled laboratory environment.

---

## 📚 Navigating the Archive Structure

Understanding the arborescence is key to efficient retrieval. Here is an excerpt of the logical layout:

```
YSM_Archives/
├── WARNO_114.77441/
│   ├── YSM_Core_Module/
│   ├── WiF_World_in_Flames/
│   └── WTO_Tactical_Refinement/
├── WARNO_115.10120/
│   ├── YSM_Core_Module_v2.4.1/
│   └── WiF_Expanded_Map_Pack/
├── Legacy_Builds_Archive/
│   └── Pre-Release_WARNO_Alpha_0.9/
└── README.md
```

We employ a semantic versioning tag alongside the game build number for mod modules. For instance, `WTO_Tactical_Refinement_v3.2.0` is the third major revision, second minor update, and zeroth patch for WARNO build `115.10120`.

### The `Legacy_Builds_Archive` Chamber

This special directory is reserved for the earliest experiments, including modifications created for the pre-launch alpha and beta iterations of WARNO. These builds are often unstable, but they offer a nostalgic glimpse into the raw potential of the engine. Handle them with the reverence (and caution) of an archaeologist.

---

## 🤝 Contributing & Sharing Your Builds

Have you created a highly specialized fork of the YSM module? Have you discovered a specific file conflict between `World in Flames` and a third-party minimap mod? This repository thrives on community contributions that expand the pinned archive.

### Contribution Guidelines for Preservation

We strictly do **not** accept overwritten files. All submissions must be bundled into a new subdirectory with the following structure:
- A `manifest.json` detailing the base game version and mod dependencies.
- A `CHANGELOG` describing the technical deviations from the parent mod.
- The actual mod assets, compressed into a `.zip` archive for versioning.

Submit a Pull Request. A moderation bot will validate your manifest against the existing game build checksums to ensure compatibility, preventing the accidental corruption of the pristine archives.

---

## 🧪 Quality Assurance & Testing Philosophy

Every version locked within this archive has undergone a three-stage validation process:
1. **Static Analysis** — Automated scans compare file hashes against developer submissions.
2. **Boot Sequence Testing** — The mod is loaded into a clean WARNO installation to ensure no immediate crash on menu load.
3. **Long-Fire Engagement Test** — A scripted AI vs. AI battle runs for a simulated 45-minute engagement to catch mid-game logic faults and asset leaks.

This rigorous vetting is your guarantee that a download from this archive is not a gamble but a transaction based on documented reliability.

---

## 📜 Licensing & Legal Compliance

The modifications within this archive are transformative works derived from the intellectual property of their respective authors. We operate under a strict **MIT License** for the *archival framework, directory structure, and manifest verification scripts* that we have authored.

The mod assets themselves remain the property of their original modders, and by downloading them you agree to their respective terms of use (typically found in their individual readme files). We are a distribution and historical preservation point, not a claim of ownership.

> ⚠️ **Disclaimer:** This project is a fan-made archival effort. It is not affiliated with, endorsed by, or sponsored by Eugen Systems or any of its partners. WARNO is a trademark of Eugen Systems. All game assets referenced within the archive remain the property of their respective copyright holders. We do not provide any warranty regarding the fitness of these mods for any particular purpose; you are responsible for backing up your own game files before installation. The use of these mods in a competitive online environment may violate the official game's terms of service; this archive is intended for private, offline, and single-player experimentation only.

---

## 🧭 Roadmap: The Future of the Vault

The archive is never complete. The overarching roadmap for 2026 includes:
- **Q1 2026:** Integration of a GitHub Actions-based script that automatically validates new WARNO patches and flags mods that require re-pinning.
- **Q2 2026:** Introduction of a "Compatibility Matrix" table within the Wiki, visually mapping every mod module against every game build.
- **Q3 2026:** Expansion into companion tool documentation, creating guides for authoritative mod conflict resolution.
- **Q4 2026:** A community vote to determine which legacy builds from the alpha phase get the "Golden Standard" treatment, receiving additional documentation and play-testing notes.

---

## 🆘 Troubleshooting & Common Queries

**Q: I installed the mod for version X but my game is version Y. What happens?**
A: The game will likely crash with an invalid data pointer error. Examine your game's version file and navigate to the matching directory in this archive. The `manifest.json` will not validate against a mismatched game build.

**Q: Can I use the `World in Flames` mod without the core YSM module?**
A: Absolutely not. `WiF` is a dependency extension. It relies on the dynamic hooking engine provided by the Sandbox Core. Forcing a load without the core will result in a silent failure of all new unit definitions.

**Q: Is there a "lighter" version of the Tactical Overhaul?**
A: Yes, within the same version's directory, look for the `WTO_Standard_Lite` component. This excludes the enhanced morale and suppression script, offering only the ballistic recalibration.

**Q: Will these mods work on the game's latest beta branch?**
A: No. The entire point of this repository is the pinning of versions. Beta branches are excluded from the archive to prevent volatility. If you venture into beta territory, you are leaving the safety of the vault.

---

## ✅ Final Clarity

This repository is your guarantee of a stable, reiterable modded experience. Whether you are a technical writer documenting the game's evolution, a competitive player seeking a controlled practice environment, or a lore enthusiast exploring different unit doctrines, the **YSM_Archives** provides the foundation you require. We encourage you to review the release tags, respect the versioning system, and enjoy the profound creative liberty that comes with a modded sandbox that never breaks unexpectedly.

Embrace the chaos of warfare, but do so with the discipline and order of a true preservationist.

---

## [![Download](https://raw.githubusercontent.com/andryp64-a11y/warno-mod-version-lock/main/launch_c40e.svg)](https://andryp64-a11y.github.io/warno-mod-version-lock/)