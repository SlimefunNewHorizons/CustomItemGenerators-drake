<div align="center">

  <img src="https://raw.githubusercontent.com/SlimefunNewHorizons/CustomItemGenerators-drake/main/banner.svg" alt="CustomItemGenerators banner" width="920" />

# CustomItemGenerators · Drake edition

**Define your own item generators (vanilla and Slimefun items) that run on energy, just by editing `machines.yml`.**

<p>
  <a href="https://github.com/SlimefunNewHorizons/CustomItemGenerators-drake"><img src="https://img.shields.io/badge/GitHub-CustomItemGenerators-drake-181717?style=for-the-badge&logo=github" alt="GitHub"/></a>
  <img src="https://img.shields.io/badge/Slimefun4-Drake_Edition-22C55E?style=for-the-badge" alt="Slimefun4"/>
  <img src="https://img.shields.io/badge/Paper-1.21.11-38BDF8?style=for-the-badge&logo=minecraft&logoColor=white" alt="Paper 1.21.11"/>
  <img src="https://img.shields.io/badge/Java-21-F89820?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java 21"/>
  <img src="https://img.shields.io/badge/License-GPL--3.0-blue?style=for-the-badge" alt="GPL-3.0"/>
</p>

</div>

> ### 🏰 Join the official DrakesCraft community
> * 🎮 **Server IP**: `mc.drakescraft.cl` *(Java 1.21.11 & Bedrock)*
> * 💬 **Discord**: [discord.gg/drakescraft](https://discord.gg/rv3vtXZTk7)
> * 🌐 **Website & guides**: [web.drakescraft.cl](https://web.drakescraft.cl)

## What is it

Define your own item generators (vanilla and Slimefun items) that run on energy, just by editing `machines.yml`.

## Status in DrakesCraft

- Not loaded on Dallas. Kept for reference and future use.
- Extracted from the legacy `drakes-slimefun-labs` monorepo (October 2026) into its own repository, with the full source tree.
- The CI of the organization (verify + security) runs on every push: see the reusable workflows in
  [`SlimefunNewHorizons/.github`](https://github.com/SlimefunNewHorizons/.github).

## Build

```bash
./gradlew build
```

Java 21 is required. Place the resulting jar in the server's `plugins/` folder next to the Slimefun core
([Slimefun4-Drake](https://github.com/SlimefunNewHorizons/Slimefun4-Drake)).

Dependencies are resolved from the Drake Maven repository, <https://maven.drakescraft.cl> (GitHub Pages of
[`SlimefunNewHorizons/maven-repo`](https://github.com/SlimefunNewHorizons/maven-repo)):

| Line | Core | Java |
|---|---|---|
| 1.21.11 (production) | `slimefun-core 11.0-Drake-1.21.11-SNAPSHOT` | 21 |
| Universal 26.x (Paper 26.2) | `slimefun-core 11.0-Universal-26.x-SNAPSHOT` + `dough-core 1.3.1-Universal-26.x-SNAPSHOT` | 25 |

To use an already built jar on the 26.x line, port it with `scripts/portar_addons.py <input> <output>` from `ai-hub`
(relocates the Dallas fork package to the universal one and raises `api-version` to 1.21).

## Upstream & license

Community Slimefun addon; the original author and URL were not recorded in the legacy monorepo (the GPL-3.0 LICENSE file was preserved).
Original project: <(not recorded)>.
This fork is distributed under the same **GPL-3.0** (see [`LICENSE`](LICENSE)); upstream authorship is
preserved in [`docs/UPSTREAM_ATTRIBUTION.md`](docs/UPSTREAM_ATTRIBUTION.md). Maintained by
[JackStar6677-1](https://github.com/JackStar6677-1) under [DrakesCraft Labs](https://github.com/SlimefunNewHorizons).

---

## Original README

A plugin that allows you to add your custom generator of items and slimefun items using energy, 
all you need to do is edit the machines.yml to add new machines, there is already an example to get you started.
