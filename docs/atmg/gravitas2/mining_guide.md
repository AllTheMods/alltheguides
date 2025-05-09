---
title: Mining and Prospecting in Gravitas²
description: A Guide to Finding and Extracting Resources in Gravitas²
authors:
 - Xannaeh
---

## Introduction to Mining in Gravitas²

Mining in Gravitas² is a far cry from vanilla Minecraft. Resources are not evenly distributed; instead, TerraFirmaCraft (TFC) introduces realistic geology, ore veins, and the necessity for careful prospecting. This guide will walk you through understanding mining safety, using prospecting tools, and the basics of finding the ores and minerals you need to progress.

---

## Safety First: Mining Hazards

Before you even swing a pickaxe underground, understand the dangers:

*   **Cave-ins are Real!** Many blocks in TFC, including most stone types, `Dirt`, `Gravel`, and `Sand`, are affected by gravity. Unsupported ceilings or walls in your mines **will collapse**, potentially trapping or killing you and burying your hard-won ores.
*   **`Support Beams` are Essential:** To prevent cave-ins, you **must** use `Support Beams`.
    *   **Crafting:** `Support Beams` are typically made from `Lumber` (which requires a `Saw`, a metal-tier tool).
    *   **Placement:** They must be placed correctly to provide structural integrity, often forming frames (horizontal beams supported by vertical ones). A single vertical beam offers little support on its own. Always place the base of your supports on solid, non-gravity-affected blocks like `Planks` or sturdy bedrock if exposed.
    *   **Controls:** ++shift++ + ++rbutton++ with `Support Beams` can sometimes place a single beam instead of attempting a larger structure, offering finer control (this may vary depending on pack configurations). Refer to in-game quest images or the TFC Guidebook for examples of proper support structures.
*   **Darkness & Mobs:** Standard Minecraft dangers from darkness still apply. Ensure your mining tunnels are well-lit with `Torches` to prevent mob spawns.

---

## Prospecting: Finding Ores and Minerals

In TerraFirmaCraft, you can't just dig randomly and hope to find what you need. Ores and minerals are found in large, distinct veins tied to specific rock types and elevations. Prospecting is the skill of locating these hidden veins.

### Understanding TFC Geology (The Basics)

*   **Rock Types Matter:** The world is composed of various rock layers (`Granite`, `Basalt`, `Limestone`, `Shale`, etc.). Different ores and minerals will *only* spawn in specific types of rock.
*   **Y-Levels (Elevation):** Veins also have preferred Y-level ranges where they generate.
*   **GregTech Vein Integration:** Gravitas² reworks GregTech veins to be compatible with TFC's geology. This means you'll encounter complex veins with multiple ore types, but their placement still respects TFC rock layers and elevations.
*   **Your Best Friend: The TFC Guidebook:** The in-game TFC Guidebook is indispensable. It contains sections on "Geology," "Ores and Minerals," and likely "Gregtech Veins," detailing which resources appear in which rock types and at what depths. **Consult it constantly!** *(A more detailed ore and mineral reference can also be found in Appendix A of this guide.)*

### Stage 1: Surface Clues - Small Nuggets & Exposed Veins

Your prospecting journey begins on the surface:

*   **Observation:** As you explore, keep a vigilant eye out for **small `Ore Nuggets`** (e.g., `Native Copper Nuggets`, `Malachite Nuggets`, `Cassiterite Nuggets`) scattered on the ground. These are your primary early indicators of nearby ore.
*   **What Nuggets Mean:**
    *   Small nuggets generally occur when an ore vein is nearby, often within **15 blocks horizontally and 35 blocks vertically**.
    *   If you find the center of a cluster of nuggets, it's highly probable that a larger vein is beneath you or very close by.
*   **Mark Your Map:** It is **absolutely crucial** to mark the location of these surface nuggets on your map (default `M` for JourneyMap or `B` for Antique Atlas). Even if you don't intend to mine there immediately, these markers are invaluable for later, more focused prospecting.
*   **Exposed Veins:** Occasionally, particularly in cliffsides, ravines, or along riverbeds and lake shores, larger sections of ore veins might be naturally exposed. These can often be spotted from a greater distance.

### Stage 2: Focused Searching - Prospecting Tools

When surface nuggets are exhausted, or you're searching for minerals that don't drop nuggets (like `Kaolinite` or `Graphite`), you'll need to employ specialized prospecting tools. These tools help detect hidden resources underground.

**Crafting Prospecting Tools (General):**
Most prospecting tool heads (for `Prospector's Picks`, `Drills`, etc.) are crafted via a similar process:
1.  Knap an unfired `Clay Mold` for the specific tool head (e.g., `Prospector's Pick Head Mold`).
2.  Fire the `Clay Mold` in a `Pit Kiln` to turn it into a `Ceramic Mold`.
3.  Cast the tool head using molten metal (starting with `Copper`) in the `Ceramic Mold`.
4.  Combine the metal tool head with a `Stick` in a crafting grid.

**Using Prospecting Tools:** All prospecting tools are generally used by selecting them in your hotbar and ++rbutton++ on a block. The tool will then provide feedback about resources in its detection range.

#### 1. The `Prospector's Pick` (ProPick) - For Metal Ores

*   **Purpose:** The standard and most essential tool for locating **metal ore veins**.
*   **Search Area:** Searches a **25x25x25 cube** centered on the block you click.
*   **Readings:** When used, it reports information to your action bar (the text above your hotbar) about the amount and type of **one** metal ore found within its range.
    *   **Possible Results:**
        *   "Nothing found." (This *can be a false negative*, especially with lower-tier ProPicks or if the vein is small or at the very edge of its range.)
        *   "Traces of [Ore Type]"
        *   "A small sample of [Ore Type]"
        *   "A medium sample of [Ore Type]"
        *   "A large sample of [Ore Type]"
        *   "A very large sample of [Ore Type]" (This is a strong indicator, suggesting at least 80 blocks of that ore nearby – a significant find!)
*   **How to Use Strategically:**
    1.  Begin in an area where you suspect ore (e.g., near surface nugget markers or in a rock type known to host the ore you seek).
    2.  ++rbutton++ a block on the surface (or underground as you create exploratory tunnels).
    3.  Carefully note the reading. "Traces" or "Small" might mean the vein is further away or minor. "Large" or "Very Large" indicates you're getting close.
    4.  Move a systematic distance (e.g., 5-10 blocks) in different directions from your last ping and test again. By comparing the strength of the readings, you can triangulate the approximate location of the vein's center.
*   **Important Notes for the ProPick:**
    *   A ProPick will **never report finding something if nothing is actually there** (no false positives for metal ores).
    *   However, it **may incorrectly report "Nothing found" when a vein *is* in range** (a false negative). Higher-tier ProPicks (made from better metals like `Bronze`, `Wrought Iron`, etc.) will have a lower chance of false negatives and may have a slightly larger detection range or better sensitivity.
    *   ProPicks of the same tier will consistently give identical results when used on the same block (unless ores have been mined out from the area).
    *   If multiple types of metal ores are within the ProPick's range, it will **only report one type per ping** (often the most abundant one or based on an internal priority). You might need to excavate one discovered vein to then be able to detect other, different veins in the same vicinity.

#### 2. The `Prospector's Hammer` - For Pinpointing Veins (Smaller Range)

*   **Purpose:** Designed for precision. Use this when your `Prospector's Pick` has indicated a general area with strong readings, but you're struggling to find the exact starting blocks of the vein, or if readings are strong all around you.
*   **Function:** Essentially a ProPick with a significantly smaller detection radius.
*   **Search Area:** Only searches a **13x13x13 cube** centered on the block inspected.
*   **When to Use:** Excellent for zeroing in on the edges of a vein or for navigating complex geology where multiple small veins might be close together.

#### 3. The `Prospector's Drill` - For Directional Searching

*   **Purpose:** Helpful when you have a hint of a vein but are unsure of its orientation or if it extends just beyond your current reach.
*   **Function:** Searches in a more directional, elongated pattern rather than a cube.
*   **Search Area:** Searches a **7x25x7 area**. The 25-block long axis of this search area is aligned with the face of the block you clicked, centered 10 blocks away from that clicked face.
    *   *Example:* If you ++rbutton++ the North face of a block with the `Prospector's Drill`, it will scan a 25-block long line extending North, starting 10 blocks North of the block you clicked.
*   **When to Use:** Ideal for chasing a vein that seems to be running in a particular direction or for checking if a vein continues after a fault or gap.

#### 4. The `Mineral Prospector` - For Non-Metallic Minerals

*   **Purpose:** Specifically for finding non-metallic minerals required for various crafting and building purposes, such as `Gypsum` (for Alabaster), `Kaolinite` (for Fire Clay), `Graphite` (for Fire Clay, Steel production), or `Flux` stones.
*   **Function:** A specialized version of the `Prospector's Pick`. It **only reports specific non-metallic minerals**, filtering out readings for metal ores.
*   **Search Area:** Reports minerals within a **45x45x45 cube** centered on the clicked block (a larger range than the standard ProPick).
*   **When to Use:** Essential when your priority is finding these non-metals and you want to avoid the "clutter" of metal ore readings that a standard ProPick would give.

### General Prospecting Strategy:

1.  **Scout & Map:** Thoroughly explore the surface for `Small Nuggets` and naturally exposed veins. Mark every potential site on your map.
2.  **Geological Research:** Consult your TFC Guidebook (and Appendix A of this guide) to identify which rock types and Y-levels are likely to host the ores/minerals you're seeking. Travel to areas with the correct geology.
3.  **Initial Scan (`Prospector's Pick` / `Mineral Prospector`):**
    *   For **metal ores**, return to nugget clusters or promising geological zones and use the standard `Prospector's Pick` every 10-15 blocks to get a general sense of what's present.
    *   For **non-metallic minerals**, use the `Mineral Prospector` in appropriate rock types/elevations.
4.  **Pinpoint (`Prospector's Hammer`):** Once your initial scans yield strong readings ("Large" or "Very Large" sample sizes), switch to the `Prospector's Hammer`. Use it in a tighter grid pattern around the strong readings to narrow down the exact starting blocks of the vein. Begin digging exploratory tunnels towards the most concentrated signals.
5.  **Direction Finding (`Prospector's Drill`):** If you're digging and lose the vein, or if initial ProPick readings are weak but consistently stronger in one particular direction, use the `Prospector's Drill` to "reach out" and check if the vein continues or is located further along that path.
6.  **Excavate & Secure:** Once you've located the vein, begin mining! Remember to diligently use `Support Beams` as you advance to prevent catastrophic cave-ins.

### Early Game Panning for Resources

Before you have a reliable supply of metal for prospecting tools, or if you're specifically looking for certain native metals or gems, **Panning** can be a useful early-game activity.

*   **Required Tool:** `Ceramic Pan` (Knap from `Clay` and fire in a `Pit Kiln`).
*   **Process:**
    1.  Locate **`Ore Deposits`**. These appear as distinct blocks within gravel patches, typically found at the bottom of freshwater lakes and rivers. Deposits can be for `Native Copper`, `Native Silver`, `Native Gold`, or `Cassiterite` (Tin).
        ![Ore Deposit Example](../img/gravitas2/ore_deposit_panning.png) <!-- Placeholder -->
    2.  With the `Ceramic Pan` in hand, ++rbutton++ the `Ore Deposit` block to collect material into your pan.
    3.  Stand in water (at least one block deep) with the filled pan selected and hold ++rbutton++. Your character will perform a panning animation.
    4.  After a few moments, you may be rewarded with one of the following in your inventory:
        *   A small piece of the deposit's `Ore` type (e.g., a `Native Copper Nugget`) - ~50% chance.
        *   A `Loose Rock` (of the surrounding rock type) - ~25% chance.
        *   A raw `Gem` (e.g., `Amethyst`, `Opal`) - ~1% chance. The type of gem obtained is tied to the rock type of the area where the gravel deposit was found.
*   **Utility:** Panning is a good way to get your very first `Copper` or `Tin` nuggets for casting, or to find early `Gold` and `Silver`.

### Understanding Ore Grades & Gem Hardness

*   **Ore Grades:** TFC ore blocks come in different grades: `Poor`, `Normal`, and `Rich`.
    *   When mined, `Rich` ore blocks yield more metal units than `Normal`, which in turn yield more than `Poor`.
    *   Veins will typically consist of a mix of these grades, with some veins being predominantly richer than others.
*   **Gem Hardness & Pickaxe Tiers:** Many gem-bearing ore blocks are harder than regular stone or common ores and require higher-tier pickaxes to mine them effectively (or at all).
    *   *Examples (may vary in Gravitas²):*
        *   `Pyrite`: `Copper` Pickaxe
        *   `Lapis Lazuli`, `Opal`: `Wrought Iron` Pickaxe
        *   `Amethyst`, `Emerald`, `Topaz`: `Steel` Pickaxe
        *   `Diamond`, `Ruby`, `Sapphire`: `Black Steel` Pickaxe
    *   Attempting to mine hard gems with an inadequate pickaxe will be very slow or impossible.

---

*This mining guide provides a foundation for resource acquisition in Gravitas². Successful mining requires patience, careful observation, strategic use of tools, and a good understanding of TFC's geology. Always refer to your in-game TFC Guidebook and JEI for the most up-to-date and pack-specific information.*

> Gravitas² | [CurseForge](https://legacy.curseforge.com/minecraft/modpacks/all-the-mods-gravitas2) | [Github](https://github.com/AllTheMods/Gravitas2)
