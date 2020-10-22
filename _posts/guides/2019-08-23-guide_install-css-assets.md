---
title: How to Install CS:S Assets
permalink: /guide/install-css-assets/
category: guide
tags:
  - install
  - cs:s
---

This guide will explain how to install Counter-Strike: Source assets onto Momentum Mod.

# Prerequisites
- SteamCMD ([https://developer.valvesoftware.com/wiki/SteamCMD](https://developer.valvesoftware.com/wiki/SteamCMD))

# Installing the CS:S server
Open SteamCMD.

Login as anonymous with
```login anonymous```

Make sure the server installs to an easily accesible directory with
```force_install_dir ./css```

Install the server
```app_update 232330 validate```

This will take a while, depending on your internet connection.

# Mounting the CS:S assets
1. Copy the `cstrike` folder from whereever the server is installed to (in this example the `css` directory) to `MomentumDev`
2. Open the `momentum/gameinfo.txt` file and the following line somewhere in the `SearchPaths` section

```game+mod                            |all_source_engine_paths|cstrike/cstrike_pak_dir.vpk```

This will add mount the CS:S assets to the game
