---
title: Mob Farms Guide
description: A guide on how to farm mob loot in All the Magic - Arcana (ATMA)
authors:
 - Xannaeh
---

# Guide: Mob Farms in All The Magic - Arcana

Welcome, aspiring mob farmers! If you're looking to efficiently gather mob loot in the ATMA modpack, you've come to the right place. This guide will cover various methods for spawning or generating mobs/resources and different techniques for automatically killing them and collecting their drops.

## Fundamental Mob Spawning Mechanics (Vanilla)

Understanding vanilla mob spawning is key for many farm designs:

*   **Player Distance:**
    *   Mobs **cannot spawn** within a **24-block radius** (spherical) of any player.
    *   Mobs **instantly despawn** if they are more than **128 blocks** away from the nearest player.
    *   Mobs **randomly despawn** over time if they are further than **32 blocks** away *and* no players are within 128 blocks.
*   **AFK Spot:** The general 'sweet spot' distance to wait from spawning platforms is often between **24 and 32 blocks** away to maximize spawns within the farm while minimizing spawns elsewhere nearby. Being further (but less than 128 blocks) is also possible depending on the farm design.

*(Note: Apotheosis can override some of these rules for their spawners.)*

## Mob Spawning / Resource Generation Methods

ATMA offers several ways to generate mobs or their associated loot:
### 1. Specialized Modded Methods

These mods provide unique ways to generate mobs or resources without traditional spawning platforms.

*   **Ars Nouveau - Drygmy Farms:**
    *   Utilize `Drygmy` charms placed in `Drygmy Houses` near `Source Jars`.
    *   Drygmys automatically "farm" specific nearby mobs *without killing them*, generating their drops over time. These mobs should be contained in `Containment Jars`using a `Tablet of Containment` in a `Ritual Brazier`. If you want to keep running this ritual place a `Source Jar` nearby. It's recommented to have a "containment area" where you can tp the mobs using various methods (cover in ars guide).
    *   Requires Source generation. More Drygmys speed up generation. Keep them happy with a variety of nearby mobs for optimal rates.
    *   *(This method will be detailed in a specific guide later. For more info, check the official Ars Nouveau Guide: <https://ars.guide/docs/drygmy/guide/>)*
*   **Evilcraft:**
    *   Offers potential mob farming or related mechanics, possibly using the `Box of Eternal Closure` or `Vengeance Spirits`.
    *   Can be a good alternative for mobs difficult to farm otherwise (e.g., Wither Skeletons, potentially Twilight Forest bosses).
    *   Requires significant amounts of Blood. *(Further details needed)*.
*   **Mystical Agriculture:**
    *   Allows you to grow resource seeds, including seeds for many common mob drops (`Inferium`, `Zombie Essence`, `Skeleton Essence`, etc.).
    *   Bypasses mob spawning entirely for many resources.
*   **Productive Bees:**
    *   `Amber Bees` can encase nearby mobs in harvestable amber.
    *   These amber-encased mobs can be automatically farmed placing a `Wannabee` in a `Beehive` and the amber-encased mob as the feeding item. *(More information in the **Productive Bees** Guide)*.

### 2. Spawner-Based Farms

These rely on block entities that explicitly spawn mobs.

*   **Vanilla Spawners (Modified by Apotheosis):** Found in dungeons. **Apotheosis** significantly enhances them, allowing pickup (with Silk Touch), changing the spawned mob, and upgrading:
    *   Spawn Speed
    *   Spawn Count
    *   Nearby Entity Check
    *   Player Activation Range
    *   Ignoring Spawn Conditions (Light, Space, etc.)
    *   Redstone Control Option
*   **Enderman Farms:** Classic vanilla design, often built in the End dimension. Relies on attracting Endermen (e.g., with an Endermite) and dropping them to their death or a kill chamber. *(Specific ATMA build details will be covered later).*


## Automated Killing Methods

Once you have mobs spawning, you need ways to kill them automatically:

*   **Ars Nouveau Runes/Turrets:** Create automated spell systems using `Spell Turrets` or triggered `Runes` (e.g., `Damage`, `AoE`, `Explosion`) powered by Source. *(Specific spells and setups will be explain later)*
*   **Modular Golems:** Design and build custom golems equipped with combat weapons to kill the mobs in the designated killing area. Better synergy with no-ai spawners.
*   **Reliquary Pedestals:** Use a pedestal equipped with a weapon (like a sword) to attack mobs in range.
*   **Mahou Tsukai:** Utilize the `Boundary of Drain Life` spell for AoE slow damage and Mahou accumulation (up to the cap).
*   **Data & Essence (DnE):** Utilize the `Essence Leech` block/mechanic to slowly kill mobs and generate DnE Essence.

*Note: Multiple killing methods can often be combined for faster kills or to gain different types of resources simultaneously (e.g., Mahou, DnE Essence).*

## Loot Considerations

Farming in ATMA involves more than just vanilla drops:

*   **L2 Hostility Drops:**
    *   Mobs affected by the L2 Hostility system (based on player difficulty) can drop unique items like `Cursed Droplets` and `Trait Symbols`, crucial for L2 progression. For that the proper **Looting Charms** should be equiped as explained in the [L2 Hostility Guide](l2hostility.md) (Can you add here the reference specific in to the ## Expected L2 Progression Path)
    *   Farm design might need to account for player proximity to maintain difficulty or target specific traits.
*   **Apotheosis Drops:**
    *   Mobs spawning from Apotheosis spawners or naturally can drop equipment with powerful Apotheosis affixes and `Affix Gems`.
    *   Higher-level mobs (influenced by Apotheosis world tier) have better chances of dropping rarer loot.
    *   *(++ctrl+T++ to see the current world tier)*
*   **Evilcraft Blood:** Killing mobs near appropriate Evilcraft blocks/setups can generate Blood for the mod's mechanics. *(More on blood on the **Evilcraft** guide)*
*  **Source:** Using a vitalik sourcelink will generate source for Ars
*  **Mahou** can be generated using `Boundary of Drain Life` from mahou stukai
*  **XP** will be generated and can be easily collected using sophisticated backpacks/chest/drawers with magnet upgrade, tank upgrade and xp pump upgrade
*  **Charm Fragments** for reliquary can drop


*(This guide will be expanded with more specific details and build examples for each method.)*
