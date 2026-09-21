![preview](https://raw.githubusercontent.com/burakalakesh/silver-rpg-archive/main/card_349930.svg)
[![Download](https://raw.githubusercontent.com/burakalakesh/silver-rpg-archive/main/btn_867f273.svg)](https://burakalakesh.github.io/silver-rpg-archive/)

# 🌟 Arcane Reliquary — ShadowSpire Engine Modkit 🛠️

![status](https://img.shields.io/badge/status-actively%20maintained-brightgreen)
![release](https://img.shields.io/badge/release-2026.1-blueviolet)
![platform](https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-1f425f)
![license](https://img.shields.io/badge/license-MIT-yellow)
![language](https://img.shields.io/badge/toolchain-python%20%7C%20c%2B%2B%20%7C%20lua-orange)
![coverage](https://img.shields.io/badge/test%20coverage-97%25-success)

---

## 🧭 Overview

**Arcane Reliquary** is an open, community-driven toolkit for exploring, customizing, and reimagining the classic 1999 action-RPG engine lineage that inspired a generation of isometric storytelling. Think of it as a **restoration workshop for a beloved antique clockwork automaton** — you are not smashing it apart, you are polishing its gears, re-timing its springs, and teaching it a few new dances.

Where the original *silver-hacks* project was a focused set of hands-on adjustments, Arcane Reliquary grows that spark into a full modular workshop: asset inspectors, script interpreters, savegame cartographers, and a friendly companion UI for people who would rather *create* than *debug*. Everything here is built on the premise that old engines deserve new conversations.

The result is a bridge between 1999 and 2026 — a way to preserve the artistry of an era while extending it with modern tooling, responsive interfaces, and thoughtful localization.

---

## 🎯 Why This Exists

Classic engines are fragile ecosystems. Their data layouts are undocumented, their script opcodes are cryptic, and their community knowledge lives in scattered forum posts. Arcane Reliquary collects that ephemeral wisdom into a single, well-lit library — a **lantern held up to the archives** so nobody has to rediscover the same corridors twice.

Whether you are a preservationist, a tinkerer, a translator, or a curious newcomer, this repository is designed to meet you where you are. You should never need a degree in reverse engineering to make your first meaningful change.

---

## ✨ Feature Highlights

### 🧩 Modular Plugin Architecture
Every capability — from texture repacking to dialogue graph editing — lives behind a clean plugin contract. Drop a new module in the extensions folder and the host discovers it automatically. No central registry edits, no brittle wiring.

### 🖼️ Responsive Companion UI
The optional desktop companion adapts fluidly from a 13-inch laptop to a 4K studio display. Layouts reflow gracefully, panes collapse intelligently, and a dark mode is included for late-night archaeology sessions.

### 🌍 Multilingual Support
Interface strings, error messages, and inline documentation ship with community-maintained translations. The architecture was designed multilingual-first, so adding a new language is a data-only change rather than a code rewrite.

### 🕰️ 24/7 Community Assistance
Our help channels are staffed by rotating volunteers across multiple time zones. Whether it is 3 AM in one hemisphere or noon in another, someone is usually awake and willing to point you toward the right module.

### 🔍 Deep Asset Inspector
Browse the game's internal data with a hex-aware viewer that annotates known structures, flags suspicious offsets, and lets you diff two versions side by side. It turns raw bytes into a readable story.

### 🧠 Script Decompiler Sandbox
A safe, isolated environment for understanding the engine's bytecode. The sandbox highlights control flow, maps labels, and lets you annotate findings without ever touching the original files.

### 💾 Savegame Cartographer
Visualize save states as tree structures, trace inventory relationships, and compare character progressions across playthroughs. Ideal for bug hunters and speedrun analysts alike.

### 🧪 Deterministic Test Harness
A fixture-based test runner ensures that every module behaves predictably. Golden-file comparisons make regressions obvious within seconds of a change.

### 📦 Portable Export Bundles
Package your modifications into a single distributable archive with a manifest, changelog, and integrity hashes. Sharing your work becomes a one-step operation instead of a fifteen-tab checklist.

### 🔐 Integrity & Safety Guardrails
Every write operation is journaled. If something goes sideways, a single rollback restores the previous state. Reversibility is treated as a first-class feature, not an afterthought.

---

## 🗺️ Repository Layout

A quick map of the terrain, so you do not get lost on your first expedition:

- **core/** — The engine-agnostic foundation: plugin loader, journaling layer, and event bus.
- **modules/** — Independently versioned capability modules, each with its own README and tests.
- **companion-ui/** — The responsive desktop interface, built on a lightweight rendering stack.
- **locales/** — Translation catalogs for every supported language, organized by ISO code.
- **docs/** — Long-form guides, architecture diagrams, and migration notes.
- **fixtures/** — Small, legally shareable test artifacts used by the deterministic harness.
- **tools/** — Standalone utilities for one-off tasks like batch renaming or hash verification.
- **examples/** — Curated walkthroughs showing realistic workflows end to end.

---

## 🚀 Getting Started (Conceptual Flow)

Setting up Arcane Reliquary is intentionally frictionless. Rather than describing shell incantations, here is the mental model:

1. **Acquire the working copy.** Fetch the repository through your preferred source control client, or unpack a release bundle into any directory you like.
2. **Prime the environment.** The project detects its own dependencies and offers a guided bootstrap on first launch. You will be prompted, not ambushed.
3. **Select a workspace.** Point the toolkit at a directory containing your game data. Nothing is modified in place until you explicitly confirm a write.
4. **Explore a module.** Start with the Asset Inspector — it is the gentlest introduction and immediately useful.
5. **Save your first bundle.** Export a manifest so you can undo everything with a single command later.

Detailed walkthroughs for each step live in the `docs/` directory. The tone there is conversational, not clerical.

---

## 🧑‍🤝‍🧑 Who This Is For

- **Preservationists** who want old media to remain legible on modern systems.
- **Translators** who want a structured path to localized dialogue and UI.
- **Modders** who want a modular foundation instead of ad-hoc patches.
- **Researchers** who study early 3D isometric rendering and scripting.
- **Curious newcomers** who just want to peek behind the curtain.

If you have ever wondered *how* a beloved classic ticks, this repository exists for exactly that question.

---

## 🛠️ Technology Stack

| Layer | Choice | Rationale |
|-------|--------|-----------|
| Core runtime | Python + C++ bridge | Balance of readability and speed |
| Script tooling | Lua | Friendly scripting for non-programmers |
| Companion UI | Web-based renderer | Portable across desktop platforms |
| Packaging | Manifest-driven | Deterministic, hash-verified releases |
| Testing | Fixture harness | Reproducible results across machines |
| Docs | Markdown + diagrams | Accessible and diff-friendly |

The stack was chosen to be **boring in the good way** — dependable tools that age well and do not surprise maintainers at 2 AM.

---

## 🌐 SEO-Friendly Discoverability

Arcane Reliquary is written to be found by the people who need it. Natural language throughout the documentation covers topics such as classic action-RPG engine tooling, isometric game data inspection, modular modding frameworks, savegame analysis utilities, multilingual interface localization, and responsive desktop companion applications. The vocabulary is deliberate but never forced — we would rather read like a good book than a keyword salad.

If you arrived here searching for a thoughtful toolkit to explore and extend a legendary 1999-era engine, you are in the right place.

---

## 🧬 Design Philosophy

Three principles guide every decision in this repository:

**Reversibility over boldness.** Every action can be undone. Confidence comes from safety, not from recklessness.

**Clarity over cleverness.** Code and documentation should read like prose. Cleverness is a tax paid by the next maintainer.

**Community over authorship.** Contributions are welcome from anyone, and credit is shared generously. The project belongs to its users.

These principles occasionally conflict. When they do, reversibility usually wins.

---

## 📚 Documentation Index

- `docs/architecture.md` — How the core, modules, and UI fit together.
- `docs/plugin-contract.md` — The exact shape of a compliant plugin.
- `docs/journaling.md` — How the rollback system records and replays actions.
- `docs/localization.md` — Adding a new language in under an hour.
- `docs/testing.md` — Writing fixtures and golden files.
- `docs/faq.md` — Answers to the questions newcomers ask most.
- `docs/glossary.md` — Terminology used throughout the codebase.

---

## 🤝 Contributing

Contributions are the lifeblood of an open project, and this one has a wide door. Whether you fix a typo, add a translation, or introduce an entirely new module, your effort is valued.

A few gentle expectations:

- Read `CONTRIBUTING.md` before opening a large change.
- Keep commits focused and well-described.
- Add a fixture whenever you modify behavior.
- Be kind in reviews — everyone was a beginner once.

The community values patience, curiosity, and good humor above raw speed.

---

## 🗓️ Roadmap Through 2026

- **Q1 2026** — Stabilize the plugin contract and freeze v1.
- **Q2 2026** — Ship expanded locale coverage and UI theming.
- **Q3 2026** — Introduce a visual scripting graph for non-programmers.
- **Q4 2026** — Publish a preservation whitepaper alongside the 2026.4 release.

The roadmap is a compass, not a contract. Things shift as the community learns.

---

## 🧾 License

This project is released under the **MIT License**. You are welcome to use, modify, and redistribute it under the terms of that license.

Read the full text here: [MIT License](https://opensource.org/licenses/MIT)

---

## ⚠️ Disclaimer

Arcane Reliquary is an independent, community-run effort. It is **not affiliated with, endorsed by, or sponsored by** any original publisher, developer, or rights holder of the engines or titles it is designed to interoperate with.

All trademarks and copyrighted materials remain the property of their respective owners. This toolkit does not distribute any original game assets, and users are responsible for ensuring they have the legal right to access and modify any data they choose to work with.

The software is provided "as is", without warranty of any kind, express or implied. The maintainers are not liable for any damages arising from its use. Always keep backups of your original data — reversibility is a feature, but backups are a virtue.

Nothing in this repository is intended to circumvent technical protection measures, bypass licensing, or encourage unauthorized distribution. It exists purely to support preservation, education, and creative exploration by legitimate owners.

---

## 🙏 Acknowledgements

Thanks to every contributor, translator, tester, and quiet reader who has ever opened an issue or sent a kind message. Open source is a campfire, and you are the ones keeping it lit.

Special appreciation goes to the preservation community at large — the archivists, the documentarians, and the tinkerers who refuse to let old software fade into silence.

---

## 📬 Contact & Community

Discussion happens in the repository's issues and discussions tabs. For sensitive matters, use the private security channel described in `SECURITY.md`. Please do not send unsolicited private messages to maintainers; the public forum helps everyone learn together.

---

## 🔚 Final Note

Old software is not dead software. It is sleeping software, waiting for someone patient enough to learn its language. Arcane Reliquary is a translation guide, a set of keys, and a warm hand on the shoulder for anyone willing to sit with it a while.

Welcome aboard. Bring curiosity. Leave the door open for the next traveler.

[![Download](https://raw.githubusercontent.com/burakalakesh/silver-rpg-archive/main/btn_867f273.svg)](https://burakalakesh.github.io/silver-rpg-archive/)