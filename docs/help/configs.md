---
title: Configs
description: What/Where are they? Customize your game!
---

# Configs

Pack configs are usually located in the `config/` folder, though others may be in your `world/serverconfigs/` folder.

!!! Warning "When editing configs, please make sure server / client is not running"

    For clients, it's safe to edit `world/serverconfigs/` while not in the world and or restarting entire client.

---

## FTB

### [FTB Essentials](https://legacy.curseforge.com/minecraft/mc-mods/ftb-essentials-forge)

Provide a couple of **Bukkit** / **Spigot** _Essentials_ like commands. `/home`, `/back`, `/tpa`, `/warp`, etc. Commands can be enabled / disabled and configured, such as cool-downs and limits, even with [FTBRanks](#ftbranks).

> **Config**: `world/serverconfig/ftbessentials.snbt`

### [FTBRanks](https://legacy.curseforge.com/minecraft/mc-mods/ftb-ranks-forge)

Includes ranks (_hence name_), is alike **Group Manager**, **EssentialsEX**, **PermX**, **LuckyPerms**, allowing you to setup custom / styled ranks for players that give additional command usages.

More information can be found on FTB Wiki: [FTBRanks](https://feedthebeast.notion.site/FTB-Ranks-d56ec50cfa04412485ff0bf63d103b4d), [FTB Essentials](https://feedthebeast.notion.site/FTB-Essentials-f1650e409e91416d941d3167f9ec89f4)

> **Config**: `world/serverconfig/ftbranks/ranks.snbt`



## [No Fly Zone](https://legacy.curseforge.com/minecraft/mc-mods/no-fly-zone)

In [ATM9](../atm9/README.md), a new mod was introduced to prohibit flight in certain dimensions.  This can be disabled.

> **Config**: `world/serverconfig/noflyzone.snbt`

## F.A.Q

??? Question "Can you make ATM ores minable by quarry?"

    By design, fake players are not allowed to mine ATM ores. This ruins the purpose of the ore being obtained naturally, thus did not come with a config to change.