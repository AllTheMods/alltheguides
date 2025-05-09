---
title: Chapter 1 - First Steps into Gravitas²
description: A Beginner's Guide to Surviving and Thriving in Gravitas² - Chapter 1
authors:
 - Xannaeh
---

## Welcome to Gravitas²!

Everything is different in Gravitas², largely thanks to **TerraFirmaCraft (TFC)**. You are about to undergo a much more realistic progression. Don't worry, this guide (and the in-game quests) are here to help you. If you ever get lost or don't know what to do, reading through this guide and the in-game quest book (often accessible via a keybind, check your controls!) should point you in the right direction.

---


## Safety First: Mining

*   **Cave-ins are real!** Mining is dangerous as caves can collapse and kill you.
*   **`Support Beams`:** To prevent cave-ins, use `Support Beams` (made from `Lumber` once you have a `Saw`).
    *   They must be placed correctly (often in a frame structure, not just single vertical beams). Place them on solid, non-gravity blocks like `Planks` or sturdy stone.
    *   ++shift++ + ++rbutton++ with `Support Beams` can place 1 instead of 3 if you need finer control (or vice-versa, depending on the pack's TFC tweak). Refer to the quest book image for an example setup.

---

## Prospecting: Finding Ores and Minerals

In TerraFirmaCraft, finding the resources you need involves more than just stumbling into a cave. You need to actively search for them using a combination of observation and specialized tools.

### Stage 1: Surface Clues - Small Nuggets

*   **Observation:** As you explore, keep an eye out for **small `Ore Nuggets`** (e.g., `Native Copper`, `Malachite`, `Tetrahedrite` for copper) scattered on the surface. These are your first indication of nearby ore.
*   **What They Mean:**
    *   Small nuggets generally occur when an ore vein is nearby, often within **15 blocks horizontally and 35 blocks vertically**.
    *   If you find the center of a group of nuggets, it's likely that a larger vein is beneath you or very close by.
*   **Mark Your Map:** It is absolutely crucial to **mark the location of these surface nuggets** on your map (`M` or `B` key). Even if you don't mine them immediately, these markers are invaluable for later, more focused prospecting.
*   **Exposed Veins:** Sometimes, larger sections of ore veins can be exposed in cliffsides or along water bodies (rivers, lakes). These can be spotted from farther away.

### Stage 2: Focused Searching - Prospecting Tools

When picking up surface nuggets becomes insufficient or you need specific non-metallic minerals, it's time to use prospecting tools. These tools help you detect hidden resources underground. All prospecting tools are used by ++rbutton++ on a block.

#### 1. The `Prospector's Pick` (ProPick) - For Metal Ores

*   **Purpose:** The standard tool for locating **metal ore veins** (which often don't have surface nuggets, or the nuggets have been exhausted).
*   **Search Area:** Searches a **25x25x25 area** centered on the block you click.
*   **Readings:** When used, it reports to your action bar (the text above your hotbar) the amount and type of **one** ore found in range.
    *   **Possible Results:**
        *   "Nothing found." (This *may* be a false negative, especially with lower-tier ProPicks or if the vein is small/far.)
        *   "Traces of [Ore Type]"
        *   "Small sample of [Ore Type]"
        *   "Medium sample of [Ore Type]"
        *   "Large sample of [Ore Type]"
        *   "Very large sample of [Ore Type]" (Indicates at least 80 blocks of ore, a significant find!)
*   **How to Use:**
    1.  Go to an area where you suspect ore (e.g., near surface nugget markers).
    2.  ++rbutton++ a block on the surface (or underground as you dig).
    3.  Note the reading. If it's "Traces" or "Small," the vein is likely further away or smaller. "Large" or "Very Large" means you're close.
    4.  Move a few blocks (e.g., 5-10 blocks) in different directions and test again. Triangulate the location of the strongest readings to pinpoint the vein.
*   **Important Notes:**
    *   A ProPick will **never report finding something when nothing is actually there**.
    *   However, it **may incorrectly say nothing is there when a vein *is* in range** (false negative). Higher-tier ProPicks (made from better metals) will reduce or eliminate these false negatives.
    *   ProPicks of the same tier will give identical results when used on the same block (unless ores were removed).
    *   If the ProPick finds multiple ore types nearby, it will **only report one** (often the most abundant or a prioritized one). You may need to dig out one vein to then detect others in the same area.

#### 2. The `Prospector's Hammer` - For Pinpointing Veins (Smaller Range)

*   **Purpose:** When you've found a general area with a ProPick but are having trouble pinpointing the exact start of the vein, or if you're in a dense area with multiple overlapping signals.
*   **Function:** A "near copy" of the ProPick but with a much smaller search range.
*   **Search Area:** Only searches a **13x13x13 area** centered on the block inspected.
*   **When to Use:** Very useful for finding the exact edges of veins that your larger ProPick has already detected. Good for when the ProPick readings seem to be "all around you."

#### 3. The `Prospector's Drill` - For Directional Searching

*   **Purpose:** If you're unsure which direction a vein extends or where it's located relative to your current position.
*   **Function:** Searches in a more directional, elongated area.
*   **Search Area:** Searches a **7x25x7 area**, with the long (25-block) side being in-line with the side of the block you clicked, centered 10 blocks away from that clicked face.
    *   For example, if you click the North face of a block, it will search a 25-block long line extending North from a point 10 blocks North of where you clicked.
*   **When to Use:** When you have a hint of a vein but need to determine its orientation or if it's just out of reach of your standard ProPick in a particular direction.

#### 4. The `Mineral Prospector` - For Non-Metallic Minerals

*   **Purpose:** If you're tired of finding metals when you need non-metallic minerals like `Gypsum`, `Kaolinite` (for Kaolin Clay), or `Graphite` (for Blast Furnaces later), this is the tool.
*   **Function:** A variation of the `Prospector's Pick`. Instead of reporting *any* nearby ores, it **only reports specific non-metallic minerals**.
*   **Search Area:** Reports minerals in a **45x45x45 area** centered on the clicked block.
*   **When to Use:** Use this when you are specifically hunting for building materials, flux components, or other non-ore minerals and want to filter out the noise of metal ore readings.


### General Prospecting Strategy:

1.  **Scout:** Explore the surface for `Small Nuggets` and exposed veins. Mark everything on your map.
2.  **Initial Scan (ProPick):** Return to areas with nugget clusters. Use the standard `Prospector's Pick` every 10-15 blocks to get a general idea of what metal ores are present and their rough locations.
3.  **Mineral Hunt (Mineral Prospector):** If specifically looking for non-metals, switch to the `Mineral Prospector` in promising geological areas.
4.  **Pinpoint (Prospector's Hammer):** Once your ProPick gives strong readings ("Large" or "Very Large"), switch to the `Prospector's Hammer` to narrow down the exact blocks where the vein starts. Dig exploratory tunnels towards the strongest readings.
5.  **Direction Find (Prospector's Drill):** If you're digging and lose the vein, or if initial ProPick readings are weak but consistent in one direction, use the `Prospector's Drill` to "reach out" and see if the vein continues.
6.  **Dig & Secure:** Once you find the vein, start mining! Remember to use `Support Beams` to prevent cave-ins.


---

*This guide is based on TerraFirmaCraft mechanics and information from the Gravitas² quest book. Specifics can vary. Always check JEI for recipes and consult your in-game TFC Guidebook!*

> Gravitas² | [CurseForge](https://legacy.curseforge.com/minecraft/modpacks/all-the-mods-gravitas2) | [Github](https://github.com/AllTheMods/Gravitas2)
