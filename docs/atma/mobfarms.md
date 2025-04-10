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

*(Note: Apotheosis can override some of these rules for its spawners.)*

## Mob Spawning / Resource Generation Methods

ATMA offers several ways to generate mobs or their associated loot:

### 1. Specialized Modded Methods

These mods provide unique ways to generate mobs or resources without traditional spawning platforms.

*   **Ars Nouveau - Drygmy Farms:**
    *   Utilize `Drygmy` charms placed in `Drygmy Houses` near `Source Jars`.
    *   Drygmys automatically "farm" specific nearby mobs *without killing them*, generating their drops over time.
    *   Mobs should be contained nearby, ideally in `Containment Jars` (captured using a `Tablet of Containment` in a `Ritual Brazier` - place a `Source Jar` nearby to sustain the ritual). A dedicated "containment area" with teleportation methods is recommended.
    *   Requires Source generation. More Drygmys speed up generation. Keep them happy with a variety of nearby mobs for optimal rates.
    *   *(This method will be detailed in a specific guide later. For more info, check the official Ars Nouveau Guide: <https://ars.guide/docs/drygmy/guide/>)*
*   **Evilcraft:**
    *   Offers potential mob farming using the `Box of Eternal Closure` with a `Vengeance Spirit` inside a `Spirit Furnace`.
    *   Can be a good alternative for mobs difficult to farm otherwise (e.g., Withers, Twilight Forest bosses).
    *   Requires significant amounts of Blood.
    *   *(This method will be detailed in a specific guide later. For the moment, you can check the in-game **Evilcraft** Guide `Origins of Darkness`)*.
*   **Mystical Agriculture:**
    *   Allows you to grow resource seeds, including seeds for many common mob drops (`Inferium`, `Zombie Essence`, `Skeleton Essence`, etc.).
*   **Productive Bees:**
    *   `Amber Bees` can encase nearby mobs in harvestable amber blocks.
    *   Place a `Wannabee` addon in a `Beehive` and feed it the amber-encased mob block to automatically "farm" drops from that mob type over time.
    *   *(This method will be detailed in a specific guide later. For the moment, you can check the in-game **Productive Bees** Guide `Big Book of Bees`. You can also refer to the [ATM9 - Productive Bees Guide](../atm9/productivebees.md) for more information on bees)*.

### 2. Spawner-Based Farms

These rely on block entities that explicitly spawn mobs or vanilla mechanics.

*   **Apotheosis Spawners:** Found in dungeons or crafted. **Apotheosis** significantly enhances vanilla spawners, allowing pickup (with Silk Touch) and changing the spawned mob with a spawn egg (use the `Capturing` enchantment to get the egg). You can modify their behavior by right-clicking the spawner with specific items:

    | Upgrade Item           | Effect                                                                                                                                                                                                 |
    | :--------------------- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | `Sugar`                | -10 Ticks Minimum Spawn Delay                                                                                                                                                                          |
    | `Clock`                | -20 Ticks Maximum Spawn Delay                                                                                                                                                                          |
    | `Fermented Spider Eye` | +2 Spawn Count (Mobs per spawn event)                                                                                                                                                                  |
    | `Ghast Tear`           | +2 Max Nearby Entities (Limit before stopping spawns)                                                                                                                                                  |
    | `Prismarine Crystal`   | +4 Blocks Player Activation Range                                                                                                                                                                      |
    | `Nether Star`          | +Ignore Players Condition (Spawns regardless of players)                                                                                                                                               |
    | `Soul Lantern`         | +Ignore Light Condition                                                                                                                                                                                |
    | `Conduit`              | +Ignore Conditions (Light, Space, etc.)                                                                                                                                                                |
    | `Echo Shard`           | +Echoing (Mobs drop extra loot)                                                                                                                                                                        |
    | `Campfire`             | +Burning (Mobs spawn on fire)                                                                                                                                                                          |
    | `Comparator`           | +Redstone Control (Requires signal to spawn). For wireless activating the redstone u can use **Create** `Redstone Link` (best option) or **Ars Nouveau** `Redstone Realy` (works within certain range) |
    | `Turtle Egg`           | +Youthful (Spawns babies if possible)                                                                                                                                                                  |
    | `Piston`               | +2 Blocks Spawn Range (Area around spawner mobs appear)                                                                                                                                                |
    | `Wool`                 | +Silent (No spawning sound)                                                                                                                                                                            |
    | `Chorus Fruit`         | +No AI (Mobs spawn without AI, good for kill chambers)                                                                                                                                                 |
    | `Pointed Dripstone`    | -5% Initial Health                                                                                                                                                                                     |

    *Note: Holding `Quartz` in your off-hand while clicking with an upgrade item will **invert** its effect (e.g., Quartz + Sugar = +10 Ticks Minimum Spawn Delay).
    For more information on the Apotheosis spawners, you can check the quest line or use JEI/EMI.*

*   `Source Spawners` from **Ars Nouveau**: They can be used to farm a designated mob located in a `Containment Jar` under the spawner. Require Source. Cannot be upgraded like **Apotheosis** ones. Might be easy to use for farming specific mobs for which you do not have the spawn egg.
*   **Enderman Farms:** Classic vanilla design, often built in the End dimension. Relies on attracting Endermen (e.g., with an Endermite) and dropping them to their death or a kill chamber. *(Specific ATMA build details will be covered later).*

## Ways To Move The Mobs

Once you have mobs spawning, you may need to move them to a comfortable killing area, potentially even across dimensions. Here are some methods:

*   **Vanilla:** Use water or lava streams to push mobs. Remember water and lava flow distance limits and that water cannot be placed in the Nether.
*   **Ars Nouveau:** `Warp Portal` blocks and `Warp Scrolls` can teleport entities.
*   **Ars Nouveau:** Use the `Glyph of Summon Decoy` to summon a decoy, trap it in a `Containment Jar`, and place the jar where you want mobs (with AI) to move towards.
*   **Ars Nouveau:** Activate a `Ritual of Attraction` in a `Ritual Brazier` and feed it with Source. This will attract mobs within an 8-block radius *(verification needed on continuous Source feeding)*.
*   **Primal Magick:** A `Zephyr Engine` will push mobs away from the direction it faces. A `Void Turbine` will pull mobs towards the direction it faces.
*   **Reactive:** *(Investigation needed)* - This mod might offer mob manipulation tools.
*   **Create:** An `Encased Fan` will push or pull mobs depending on the direction of its rotational force.
*   *(Other potential methods like Create contraptions, pedestals, etc., could be added here)*

### Setup Examples (Mob Movement)

=== "Vanilla"

    *(Example + images go here)*

=== "Ars Nouveau Warp Portal"

    First, you need to set up the area where you want to kill the mobs. I recommend at least a 2x2 to avoid mob clipping. Then with a `Warp Scroll` (for the same dimension movement) or a `Stabilized Warp Scroll` (for interdimesnion movement) in your hand ++shift+right-button++ in the middle of that area to set the teleportation destination.
    ![Killing Area](img/mobfarms/ars_wp_killing_area.png)
    After that, you need to build up the place where the mobs will be spawning. The portal characteristics should be based on the `Spawner` spawn range. The first layer should be any solid block (where mobs will spawn), then make a border with `Sourcestone`, `Mirrorweave` or `Ghostweave` (the last two can change the apperance to any block in the game), on top of that border you can either place slabs, leaves with water (useful for endermen) or simply make a solid wall. The spawner should be elevated in the middle of the platform depending on the spawn range of your spawner (to avoid having mobs spawning below the portal), as well as have solid blocks placed on top of the spawner to avoid mobs getting stuck in there.
    ![Portal Setup](img/mobfarms/ars_wp_portal_setup.png)
    For activating the portal you need to have a source jar nearby and throw the scroll that you configured before linked to the killing area.
    ![Portal Activation](img/mobfarms/ars_wp_portal_activation.png)
    With that you will have the mobs getting spawned in one place and dimension (so you can benefit of exclusive drops from certain dimensions) and kill them wherever you prefer.


=== "Ars Nouveau Decoy"

    *(Example + images go here)*

=== "Ars Nouveau Ritual of Attraction"

    *(Example + images go here)*

=== "Primal Magick"

    *(Example + images go here)*

=== "Reactive"

    *(Example + images go here)*

=== "Create"

    *(Example + images go here)*

## Automated Killing Methods

Once you have the mobs in place, you need ways to kill them automatically:

*   **Ars Nouveau Runes/Turrets:** Create automated spell systems using `Spell Turrets` or triggered `Runes` (e.g., `Damage`, `AoE`, `Explosion`) powered by Source. *(Specific spells and setups will be explained later)*.
*   **Modular Golems:** Design and build custom golems equipped with combat weapons (`Melee Module`, `Ranged Module`) to kill mobs in a designated area. Works particularly well with spawners set to ignore AI (`No AI` upgrade).
*   **Reliquary Pedestals:** Use a pedestal equipped with a weapon (like a sword) to attack mobs in range.
*   **Mahou Tsukai:** Utilize the `Boundary of Drain Life` spell for AoE slow damage and Mahou accumulation (up to the cap).
*   **Data & Essence (DnE):** Utilize the `Essence Leech` block/mechanic to slowly kill mobs and generate DnE Essence.
*   **Data & Essence (DnE):** Utilize a `Laser Emitter` with a specific lens depending on your needs:
    *   `Harming Lens`: General damage.
    *   `Burning Lens`: Sets mobs on fire.

*Note: Multiple killing methods can often be combined for faster kills or to gain different types of resources simultaneously (e.g., Mahou, DnE Essence).*

### Setup Examples (Killing Methods)

=== "Ars Nouveau Runes"

    *(Example + images go here)*

=== "Ars Nouveau Turrets"

    *(Example + images go here)*

=== "Modular Golems"

    *(Example + images go here)*

=== "Reliquiary Pedestals"

    *(Example + images go here)*

=== "Mahou Tsukai"

    *(Example + images go here)*

=== "Data and Essence Leech"

    *(Example + images go here)*

=== "Data and Essence Lasers"

    *(Example + images go here)*


=== "Combination of Methods"

    *(Example + images go here)*


## Loot Considerations & Extra Resources

Farming in ATMA involves more than just vanilla drops. Consider these potential outputs:

*   **L2 Hostility Drops:**
    *   Mobs affected by the L2 Hostility system (based on player difficulty) can drop unique items like `Cursed Droplets` and `Trait Symbols`, crucial for L2 progression.
    *   Ensure the appropriate **Looting Charms** are equipped, as explained in the [L2 Hostility Guide > Expected Progression](l2hostility.md#expected-l2-progression-path).
    *   Farm design might need to account for player proximity to maintain difficulty or target specific traits.
*   **Apotheosis Drops:**
    *   Mobs spawning from Apotheosis spawners or naturally can drop equipment with powerful Apotheosis affixes and `Affix Gems`.
    *   Higher-level mobs (influenced by Apotheosis world tier) have better chances of dropping rarer loot.
    *   *(Press ++ctrl+t++ (default keybind) to see the current world tier)*.
*   **Evilcraft Blood:** Killing mobs near appropriate Evilcraft blocks/setups can generate Blood for the mod's mechanics. *(More on blood generation in the **Evilcraft** guide)*.
*   **Ars Nouveau Source:** Using a `Vitalic Sourcelink` near a killing area can generate Source from mob deaths.
*   **Data and Essence Essence:** Using a `Essence Leech` in the killing area will slowly drain essence from the mobs.
*   **Mahou Tsukai Mahou:** Can be generated using the `Boundary of Drain Life` killing method.
*   **Experience (XP):** Mobs drop XP orbs, which can be collected using:
    *   **Sophisticated Storage:** `Magnet Upgrade`, `Tank Upgrade`, and `XP Pump Upgrade` on backpacks, chests, or barrels.
    *   *(Other collection methods like Experience Pylons, Absorption Hoppers, etc.)*
*   **Reliquary Charm Fragments:** Can occasionally drop from mobs.
*   **Occultism mobs** can be also farmed in spawners and with drygmes. Just beaware that rituals that **Occultism* `Wild Breeze` (the 3 levels of it) spawners spawn multiple mobs, not only the breeze and to that mobs the NO AI from Apotheoisis doenst apply. Drygme farm is recommended for `Wild Breeze` farming.

*(This guide will be expanded with more specific details and build examples for each method.)*
