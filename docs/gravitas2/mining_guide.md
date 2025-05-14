---
title: Prospecting, Geology, and Mining
description: A Comprehensive Guide to Finding and Extracting Resources in Gravitas²
authors:
 - Xannaeh
---

## Introduction to Mining in Gravitas²

Mining in Gravitas² is a far cry from vanilla Minecraft. Resources are not evenly distributed; instead, TerraFirmaCraft (TFC) introduces realistic geology, ore veins, and the necessity for careful prospecting. This guide will walk you through understanding mining safety, TFC geology, using prospecting tools, and locating the specific ores and minerals you need to progress.

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

## Understanding TerraFirmaCraft Geology

The world of TerraFirmaCraft is structured with distinct geological features that dictate where resources can be found. Knowing basic geology is key to efficient prospecting.

### A. Continents and Rock Regions
*   The world features large landmasses separated by oceans.
*   These landmasses are divided into **rock regions**, often over a kilometer across. Typically, you'll find two or three different **rock layers** under your feet at any given location.
*   Identifying the rock types present in an area is crucial, as different ores and minerals will often only appear in specific rock types.

### B. Rock Categories and Formations

TFC rocks are broadly categorized, and their formation influences where they (and associated ores) are found:

1.  **Igneous Extrusive Rocks:**
    *   Formed from magma (lava) cooling quickly on the Earth's surface.
    *   Commonly found as the top layer of rock on continents or forming the entirety of ocean floors.
    *   The type of igneous intrusive rock found *beneath* an extrusive layer is usually of the same geological "grade" (Felsic, Intermediate, Mafic).
    *   **Examples:** `Rhyolite` (Felsic), `Basalt` (Mafic), `Andesite` (Intermediate), `Dacite` (Intermediate).

2.  **Sedimentary Rocks:**
    *   Formed by the accumulation and deposition of mineral or organic particles over long periods.
    *   Typically found as the top layers of rock in continental (land) areas.
    *   When found deeper, or subjected to geological pressure, they often have corresponding metamorphic rocks beneath them.
    *   **Examples:** `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk`.

3.  **Metamorphic Rocks:**
    *   Created when existing rocks (sedimentary or igneous) are transformed by heat, pressure, or chemical reactions.
    *   Found underneath their corresponding "parent" sedimentary or igneous rocks, or brought to the surface in mountainous "uplift" regions.
    *   **Formation Examples:**
        *   `Slate` forms from `Shale`, `Claystone`, or `Conglomerate`.
        *   `Marble` forms from `Limestone`, `Dolomite`, or `Chalk`.
        *   `Quartzite` forms from `Chert` (or sandstone).
        *   `Phyllite` forms from `Slate` (further metamorphism).
        *   `Schist` and `Gneiss` form from `Phyllite` or igneous intrusive rocks (Gneiss representing a higher grade of metamorphism).

4.  **Igneous Intrusive Rocks:**
    *   Formed when magma cools slowly *beneath* the Earth's crust.
    *   Typically found deep underground. They can also be exposed at the surface in **uplift regions** (areas of intense geological activity like mountain ranges) or as **dikes** (narrow, vertical intrusions of magma that cut through other rock layers).
    *   **Examples by Grade:**
        *   *Felsic:* `Granite` (often found under `Rhyolite`).
        *   *Intermediate:* `Diorite` (often found under `Andesite` or `Dacite`).
        *   *Mafic:* `Gabbro` (often found under `Basalt`).

### C. Ore Vein Characteristics
*   Unlike vanilla Minecraft, TFC ores are found in **massive, sparse, yet often rich veins**. These veins can be hundreds of blocks long and many blocks thick.
*   **Graded Ores:** Most TFC ore blocks come in three grades: `Poor`, `Normal`, and `Rich`.
    *   `Rich` ore blocks yield the most metal units when processed.
    *   `Normal` ore blocks yield a moderate amount.
    *   `Poor` ore blocks yield the least.
    *   An ore vein will typically contain a mixture of these grades, with the overall "richness" of a vein varying.

---

## GregTech Vein Integration in Gravitas²

A significant feature of Gravitas² is the integration of **GregTech-style ore veins**, reworked to be compatible with TerraFirmaCraft's geology.
*   This means you will encounter large, multi-ore veins characteristic of GregTech, but their spawning locations (host rock types and Y-levels) will generally adhere to TFC's geological rules.
*   The in-game **TFC Guidebook** have a dedicated section that you can navigate to find information on the composition of these complex veins and the TFC rock types they are associated with. This is your primary reference for GT veins.

---

## Prospecting Tools & Techniques

Finding these hidden veins requires specific tools and a methodical approach.

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
    2.  With the `Ceramic Pan` in hand, ++rbutton++ the `Ore Deposit` block to collect material into your pan.
    3.  Stand in water (at least one block deep) with the filled pan selected and hold ++rbutton++. Your character will perform a panning animation.
    4.  After a few moments, you may be rewarded with one of the following in your inventory:
        *   A small piece of the deposit's `Ore` type (e.g., a `Native Copper Nugget`) - ~50% chance.
        *   A `Loose Rock` (of the surrounding rock type) - ~25% chance.
        *   A raw `Gem` (e.g., `Amethyst`, `Opal`) - ~1% chance. The type of gem obtained is tied to the rock type of the area where the gravel deposit was found.
*   **Utility:** Panning is a good way to get your very first `Copper` or `Tin` nuggets for casting, or to find early `Gold` and `Silver`.

---

## Using Caves and Surface Geology to Guide Prospecting

While TFC doesn't have fixed "cave layers" that directly point to specific ores like in some other mods, you can use the exposed geology of caves and surface features to make educated guesses about what might be nearby:

1.  **Identify Exposed Rock Types:** When you're on the surface or exploring a cave, pay close attention to the types of stone you see. TFC typically has 2-3 distinct rock layers stacked vertically in any given area.
2.  **Note Your Y-Level:** Your current elevation is critical.
3.  **Cross-Reference with Ore Data:** Once you know the rock type(s) and your Y-level, consult the detailed ore tables below (and your in-game TFC Guidebook). Look for ores that are known to spawn in those specific rock types and within that elevation range.
4.  **Prospect in Promising Areas:** If a cave cuts through, for example, `Granite` between Y=10 and Y=80, it's a good area to start using your `Prospector's Pick` to search for `Cassiterite Veins (GT)` or other ores known to spawn in `Granite` at those depths.
5.  **Surface Indicators (Mineral Hints & Nuggets):**
    *   **Nuggets:** Small ore nuggets on the surface are direct indicators of a metallic ore vein nearby.
    *   **Mineral Hints (OreHints):** TFC can generate "Hint Rocks" on the surface or in caves. These are small, out-of-place rocks that don't match the surrounding geology. If you find a piece of `Basalt` on a `Granite` surface, that `Basalt` could be a hint for an ore that commonly spawns *with* `Basalt` (like `Lignite` or `Bituminous Coal` according to the hint list). The "Mineral Hints" column in the tables below incorporates this information. Kaolinite's hint (Blood Lily flower) is a classic example.

By combining geological knowledge with prospecting tools, you can significantly improve your chances of finding the resources you need.

---
## Detailed Ore and Mineral Vein Reference (Gravitas² Edition)

This section provides a detailed reference for locating key ores and minerals. Vein compositions may combine TFC defaults and GregTech logic in Gravitas².

**Important Considerations Before Using These Tables:**

*   **Gravitas² Specifics:** This information is a comprehensive starting point. **Gravitas² may have custom ore generation configurations.**
*   **IN-GAME GUIDE IS KING:** **Always prioritize and cross-reference this information with your in-game TFC Guidebook (especially its "Ores and Minerals" and "Gregtech Veins" sections) and JEI (Just Enough Items).** These will provide the most accurate details for your specific pack version.
*   **Vein Naming:** (GT) denotes veins primarily from GregTech style generation. (TFC) denotes TerraFirmaCraft default veins/deposits.
*   **Mineral Hints:** The "Mineral Hint / Surface Indicator" column lists out-of-place rocks ("X pebble in Y rock") or specific plants that might indicate the presence of the ore/mineral nearby. This is based on the "OreHints" mechanic. For metallic ores, nuggets are the primary surface indicators.

---
### Copper (Cu) Ores

| Vein Name / Type      | Common Ores in This Vein (Gravitas²)                         | Y-Level Range | Host Rock Types (TFC Specific Names)                        | Mineral Hint / Surface Indicator | Notes & Tips                                                      |
|-----------------------|--------------------------------------------------------------|---------------|-------------------------------------------------------------|------------------------------------|-------------------------------------------------------------------|
| Native Copper (TFC)   | `Native Copper`                                              | y > 40        | `Rhyolite`, `Basalt`, `Andesite`, `Dacite` (Igneous Extrusive)  | `Copper Nuggets`                   | Common early copper. Also by panning.                             |
| Tetrahedrite (TFC)    | `Tetrahedrite` (Copper ore)                                  | Any           | `Quartzite`, `Slate`, `Phyllite`, `Schist`, `Gneiss`, `Marble` (Metamorphic) | `Tetrahedrite Nuggets`             | Deeper veins often richer.                                        |
| Malachite (TFC)       | `Malachite` (Copper ore)                                     | Any           | `Limestone`, `Chalk`, `Dolomite` (Sedimentary); `Marble` (Metamorphic) | `Malachite Nuggets`                | Deeper veins often larger/richer. Found with `Limestone`.         |
| Copper Vein (GT)      | `Chalcopyrite`, `Iron`, `Pyrite`, `Copper`                   | y=-40 to y=10 | `Diorite`, `Granite`                                        | `Chalcopyrite Nuggets`, `Pyrite Nuggets`    |                                                                   |
| Copper Tin Vein (GT)  | `Chalcopyrite`, `Zeolite`, `Cassiterite` (Tin), `Realgar`    | y=-10 to y=160| `Basalt`, `Rhyolite`, `Andesite`, `Dacite`                  | `Chalcopyrite Nuggets`, `Cassiterite Nuggets` | Excellent GT vein for early `Copper` and `Tin`.                   |

---
### Tin (Sn) Ores

| Vein Name / Type      | Common Ores in This Vein (Gravitas²)                         | Y-Level Range | Host Rock Types (TFC Specific Names)                           | Mineral Hint / Surface Indicator | Notes & Tips                                         |
|-----------------------|--------------------------------------------------------------|---------------|----------------------------------------------------------------|------------------------------------|------------------------------------------------------|
| Cassiterite (TFC)     | `Cassiterite` (Tin ore)                                      | y > 80        | `Granite`, `Diorite`, `Gabbro` (Igneous Intrusive in uplift/dikes) | `Cassiterite Nuggets`              | TFC default Tin. Also by panning.                    |
| Cassiterite Vein (GT) | `Tin`, `Cassiterite`                                         | y=10 to y=80  | `Granite`, `Diorite`, `Gabbro`                                 | `Cassiterite Nuggets`              |                                                      |
| Garnet Tin Vein (GT)  | `Cassiterite Sand`, `Garnet Sand`, `Asbestos`, `Diatomite`   | y=30 to y=60  | `Limestone`, `Chalk`                                           | Prospect in `Limestone`/`Chalk`. | Source of Tin and industrial minerals.             |

---
### Iron (Fe) Ores

| Vein Name / Type   | Common Ores in This Vein (Gravitas²)                               | Y-Level Range | Host Rock Types (TFC Specific Names)                                          | Mineral Hint / Surface Indicator | Notes & Tips                                           |
|--------------------|--------------------------------------------------------------------|---------------|-------------------------------------------------------------------------------|------------------------------------|--------------------------------------------------------|
| Hematite (TFC)     | `Hematite` (Iron ore)                                              | Near Surface  | `Rhyolite`, `Basalt`, `Andesite`, `Dacite` (Igneous Extrusive)                  | `Hematite Nuggets`                 | Large TFC iron veins.                                  |
| Magnetite (TFC)    | `Magnetite` (Iron ore)                                             | Near Surface  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk` (Sedimentary) | `Magnetite Nuggets`                | Large TFC iron veins.                                  |
| Limonite (TFC)     | `Limonite` (Iron ore)                                              | Near Surface  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk` (Sedimentary) | `Limonite Nuggets`                 | Large TFC iron veins.                                  |
| Iron Vein (GT)     | `Goethite`, `Yellow Limonite`, `Hematite`, `Malachite`, `Chromite` | y=-10 to y=60 | `Basalt`, `Rhyolite`, `Andesite`, `Dacite`                                    | `Hematite Nuggets`, `Limonite Nuggets`      | Diverse GT iron source, includes `Chromite`.           |
| Magnetite Vein (GT)| `Magnetite`, `Vanadium Magnetite`, `Gold`                          | y=10 to y=60  | `Basalt`, `Rhyolite`, `Andesite`, `Dacite`                                    | `Magnetite Nuggets`, `Gold Nuggets`         | GT vein, also source of `Gold` and `Vanadium`.       |

---
### Gold (Au), Silver (Ag), Lead (Pb) Ores

| Vein Name / Type      | Common Ores in This Vein (Gravitas²)                         | Y-Level Range | Host Rock Types (TFC Specific Names)                                                    | Mineral Hint / Surface Indicator | Notes & Tips                                                     |
|-----------------------|--------------------------------------------------------------|---------------|-----------------------------------------------------------------------------------------|------------------------------------|------------------------------------------------------------------|
| Native Gold (TFC)     | `Native Gold`                                                | y < 70        | `Rhyolite`, `Basalt`, `Andesite`, `Dacite` (Igneous Extrusive); `Granite`, `Diorite`, `Gabbro` (Igneous Intrusive) | `Gold Nuggets`                     | Deeper veins larger/richer. Also by panning. Often with GT Magnetite Vein. |
| Native Silver (TFC)   | `Native Silver`                                              | y > 90 (poor) or y < 20 (rich) | `Granite`, `Diorite` (uplift); `Granite`, `Diorite`, `Schist`, `Gneiss` (deep)        | `Silver Nuggets`                   | TFC default. Also by panning.                                    |
| Galena Vein (GT)      | `Galena` (Lead/Silver ore), `Silver`, `Lead`                 | y=-15 to y=45 | `Granite`, `Gneiss`                                                                     | `Galena Nuggets`                   | Primary GT Lead and Silver source.                               |

---
### Zinc (Zn), Nickel (Ni), Bismuth (Bi), Chromium (Cr) Ores

| Vein Name / Type   | Common Ores in This Vein (Gravitas²)                         | Y-Level Range | Host Rock Types (TFC Specific Names)                                                      | Mineral Hint / Surface Indicator | Notes & Tips                                       |
|--------------------|--------------------------------------------------------------|---------------|-------------------------------------------------------------------------------------------|------------------------------------|----------------------------------------------------|
| Sphalerite (TFC)   | `Sphalerite` (Zinc ore)                                      | Near surface (poor) or deep (rich) | `Rhyolite`, `Basalt`, `Andesite`, `Dacite` (Igneous Extrusive - poor); `Granite`, `Diorite`, `Gabbro` (Igneous Intrusive - rich); `Quartzite` (Metamorphic, per quest) | `Sphalerite Nuggets`               | TFC default.                                       |
| Garnierite (TFC)   | `Garnierite` (Nickel ore)                                    | y < 0         | `Gabbro` (primarily); `Granite`, `Diorite` (Igneous Intrusive - rarer)                     | `Garnierite Nuggets`               | TFC default.                                       |
| Nickel Vein (GT)   | `Garnierite`, `Nickel`, `Cobaltite`, `Pentlandite`           | y=-10 to y=60 | `Gabbro`, `Diorite`, `Granite`                                                              | `Garnierite Nuggets`               | Main GT Nickel source, includes `Cobalt`.          |
| Bismuthinite (TFC) | `Bismuthinite` (Bismuth ore)                                 | Near surface or deep | `Shale`, `Claystone`, etc. (Sedimentary - near surface); `Granite`, `Diorite`, `Gabbro` (Igneous Intrusive - deep, richer) | `Bismuthinite Nuggets`             | TFC default. Needed for `Bismuth Bronze`.        |
| Chromite (TFC Small Ore) | `Chromite`                                               | Any           | `Granite`, `Diorite`, `Gabbro` (Igneous Intrusive); `Slate`, `Phyllite`, `Schist`, `Gneiss`, `Marble` (Metamorphic) | `Small Chromite pieces` (No specific rock hint from list) | Found as small pieces, not large TFC veins.        |
| Chromite Vein (GT)   | `Chromite`, `Nickel`                                         | y=-50 to y=55 | `Granite`, `Diorite`, `Gabbro`, `Schist`, `Phyllite`                                      | `Small Chromite pieces`            | GT source of `Chromium` and some `Nickel`.         |

---
### Coal

| Vein Name / Type      | Common Ores in This Vein (Gravitas²)                         | Y-Level Range | Host Rock Types (TFC Specific Names)                                          | Mineral Hint / Surface Indicator | Notes & Tips                           |
|-----------------------|--------------------------------------------------------------|---------------|-------------------------------------------------------------------------------|------------------------------------|----------------------------------------|
| Lignite (TFC)         | `Lignite` (Low-grade coal)                                   | Near Surface  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk` (Sedimentary) | `Basalt` pebble in `Shale` or `Claystone` rock | Large, flat deposits. Fuel.            |
| Bituminous Coal (TFC) | `Bituminous Coal` (Mid-grade coal)                           | Near Surface  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk` (Sedimentary) | `Basalt` pebble in `Shale` or `Claystone` rock | Large, flat deposits. Better fuel.     |
| *Also see Diamond Vein (GT) under Gems for more Coal/Graphite.* |               |               |                                                                               |                                    |                                        |

---
### Gems & Decorative Minerals

| Vein Name / Type         | Common Ores in This Vein (Gravitas²)                         | Y-Level Range | Host Rock Types (TFC Specific Names)                                          | Mineral Hint / Surface Indicator | Notes & Tips                                                     |
|--------------------------|--------------------------------------------------------------|---------------|-------------------------------------------------------------------------------|------------------------------------|------------------------------------------------------------------|
| Diamond Vein (GT)        | `Graphite`, `Diamond`, `Coal`                                | y=-65 to y=10 | `Gabbro`                                                                      | `Chalk` pebble in `Basalt` rock or `Gabbro` rock (if uplifted) | GT Kimberlite pipes. Primary source of `Diamonds` and `Graphite`.|
| Emerald (TFC)            | `Emerald`                                                    | Any           | `Granite`, `Diorite`, `Gabbro` (Igneous Intrusive)                              | (No specific rock hint)            | Thin, tall vertical formations in TFC.                           |
| Lapis Lazuli (TFC)       | `Lapis Lazuli`                                               | y=-20 to y=80 | `Limestone`, `Marble`                                                         | `Andesite` pebble in `Limestone` rock | Large, sparse TFC veins.                                         |
| Lapis Lazuli Vein (GT)   | `Lazurite`, `Sodalite`, `Lapis`, `Calcite`                   | y=-65 to y=-30| `Basalt`, `Rhyolite`, `Andesite`, `Dacite`                                    | `Andesite` pebble in `Basalt` or `Rhyolite` rock | GT vein for Lapis and related minerals.                          |
| Garnet Vein (GT)         | `Red Garnet`, `Yellow Garnet`, `Amethyst`, `Opal`            | y=-10 to y=50 | `Granite`, `Claystone`                                                        | No single X pebble hint for this vein. Prospect in `Granite`/`Claystone`. | GT source for various gems.                                      |
| Sapphire Vein (GT)       | `Almandine`, `Pyrope`, `Sapphire`, `Green Sapphire`          | y=-40 to y=0  | `Schist`, `Quartzite`                                                         | (No specific rock hint)            | GT source for Sapphires and related garnets.                     |
| Amethyst (TFC Deposit)   | `Amethyst`                                                   | y > 40        | `Shale`, `Claystone`, etc. (Sedimentary); `Slate`, `Marble`, etc. (Metamorphic) - beneath rivers | (No specific rock hint)            | TFC default.                                                     |
| Opal (TFC Deposit)       | `Opal`                                                       | y > 40        | `Shale`, `Claystone`, etc. (Sedimentary); `Rhyolite`, `Basalt`, etc. (Igneous Extrusive) - beneath rivers | (No specific rock hint)            | TFC default.                                                     |

---
### Industrial Minerals (Non-Metallic)

| Vein Name / Type         | Common Ores in This Vein (Gravitas²)                               | Y-Level Range | Host Rock Types (TFC Specific Names)                                                                  | Mineral Hint / Surface Indicator | Notes & Tips                                                                                 |
|--------------------------|--------------------------------------------------------------------|---------------|-------------------------------------------------------------------------------------------------------|------------------------------------|----------------------------------------------------------------------------------------------|
| Apatite Vein (GT)        | `Apatite`, `Tricalcium Phosphate`, `Pyrochlore`                    | y=10 to y=80  | `Basalt`, `Rhyolite`, `Andesite`, `Dacite`, `Granite`, `Gabbro`, `Diorite`                           | (No specific rock hint)            | GT source of Phosphate (for fertilizer).                                                     |
| Salts Vein (GT)          | `Rock Salt`, `Salt`, `Lepidolite`, `Spodumene`                     | y=30 to y=70  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk`                       | `Phyllite` pebble in `Shale` or `Limestone` rock | GT source of `Salt` and Lithium (`Lepidolite`, `Spodumene`).                                 |
| Mineral Sand Vein (GT)   | `Basaltic Mineral Sand`, `Granitic Mineral Sand`, `Fullers Earth`, `Gypsum` | y=15 to y=60 | `Basalt`, `Granite`                                                                                 | For Gypsum: `Quartzite` pebble in `Basalt` rock or `Granite` rock (if uplifted) | GT source of various sands and `Gypsum`.                                                     |
| Lubricant Vein (GT)      | `Soapstone`, `Talc`, `Glauconite Sand`, `Pentlandite`              | y=0 to y=50   | `Schist`                                                                                              | (No specific rock hint)            | GT source of `Talc` (for lubrication), `Soapstone`.                                          |
| Mica Vein (GT)           | `Kyanite`, `Mica`, `Bauxite`, `Pollucite`                          | y=-40 to y=-10| `Quartzite`, `Slate`, `Phyllite`, `Schist`, `Gneiss`, `Marble`, `Gabbro`, `Diorite`, `Granite`        | (No specific rock hint)            | GT source of `Mica` and `Bauxite` (Aluminum).                                                |
| Oilsands Vein (GT)       | `Oilsands`                                                         | y=30 to y=80  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk`                       | (No specific rock hint)            | GT source of `Oil`.                                                                          |
| Kaolinite (TFC Deposit)  | `Kaolinite Clay`                                                   | High Altitudes| Special Environmental: Plateaus, Old Mountains, Highlands (Temp >= 18°C, Rainfall >= 300mm)        | `Blood Lily` Flower                | Used for Fire Clay. Not a typical "vein."                                                  |
| Graphite (TFC Deposit)   | `Graphite`                                                         | y < 60        | `Gneiss`, `Marble`, `Quartzite`, `Schist` (Metamorphic)                                               | `Claystone` pebble in `Gneiss` or `Schist` rock | Used for Fire Clay. Also found in GT Diamond Veins.                                          |
| Cinnabar (TFC Deposit)   | `Cinnabar`                                                         | Deep          | `Quartzite`, `Granite`, `Phyllite`, `Schist`                                                          | `Gneiss` pebble in `Granite` or `Schist` rock | Ground for Redstone Dust. Also in GT Redstone/Thorium veins.                                 |
| Cryolite (TFC Deposit)   | `Cryolite`                                                         | Deep          | `Granite`, `Diorite` (Igneous Intrusive)                                                              | `Slate` pebble in `Granite` or `Rhyolite` rock | Ground for Redstone Dust.                                                                    |
| Saltpeter (TFC Deposit)  | `Saltpeter`                                                        | Near Surface  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk` (Sedimentary)        | `Diorite` pebble in `Shale` or `Limestone` rock | Ground for Gunpowder. Large flat deposits.                                                   |
| Sulfur (TFC Deposit)     | `Sulfur`                                                           | Near Lava Lvl | Any Metamorphic (`Quartzite`, `Slate`, etc.) or Igneous Intrusive (`Granite`, `Diorite`, `Gabbro`) | `Shale` pebble in `Granite` or `Slate` rock | Ground for Gunpowder. Sparse but large veins.                                                |
| Sylvite (TFC Deposit)    | `Sylvite`                                                          | Near Surface  | `Shale`, `Claystone`, `Chert` (Sedimentary)                                                         | `Dolomite` pebble in `Shale` or `Chert` rock | Ground for Fertilizer. Large flat deposits.                                                  |
| Borax (TFC Deposit)      | `Borax`                                                            | Near Surface  | `Claystone`, `Limestone`, `Shale` (Sedimentary)                                                     | `Chert` pebble in `Claystone` or `Limestone` rock | Ground for Flux. Large flat deposits.                                                        |
| Gypsum (TFC Deposit)     | `Gypsum`                                                           | Near Surface  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk` (Sedimentary)        | `Quartzite` pebble in `Shale` or `Limestone` rock | Decorative (Alabaster). Large flat deposits. Also in GT Mineral Sand Veins.                  |
| Halite (TFC Deposit)     | `Halite` (Rock Salt)                                               | Near Surface  | `Shale`, `Claystone`, `Limestone`, `Conglomerate`, `Dolomite`, `Chert`, `Chalk` (Sedimentary)        | `Phyllite` pebble in `Shale` or `Limestone` rock | Ground for Salt (Preservative). Large flat deposits. Also in GT Salts Veins.                 |

---
### Radioactive & Other GregTech Specific Veins

| Vein Name / Type     | Common Ores in This Vein (Gravitas²)                               | Y-Level Range | Host Rock Types (TFC Specific Names)                                          | Mineral Hint / Surface Indicator | Notes & Tips                                                     |
|----------------------|--------------------------------------------------------------------|---------------|-------------------------------------------------------------------------------|------------------------------------|------------------------------------------------------------------|
| Thorium Vein (GT)    | `Thorium`, `Cinnabar`, `Uraninite`                                 | y=-50 to y=25 | `Basalt`, `Rhyolite`, `Dacite`, `Andesite`                                    | For Cinnabar component: `Gneiss` pebble in `Basalt` or `Rhyolite` rock | GT source for radioactive materials.                             |
| Redstone Vein (GT)   | `Redstone`, `Ruby`, `Cinnabar`, `Thorium`                          | y=-65 to y=-10| `Rhyolite`, `Basalt`, `Andesite`, `Dacite`, `Quartzite`, `Shale`              | For Cinnabar component: `Gneiss` pebble in host rock (e.g., `Rhyolite`, `Shale`, `Quartzite`) | Primary GT `Redstone` source, also `Ruby`.                       |
| Manganese Vein (GT)  | `Grossular`, `Spessartine`, `Pyrolusite` (Manganese), `Tantalite`   | y=-30 to y=0  | `Phyllite`, `Granite`, `Quartzite`                                            | (No specific rock hint)            | GT source of `Manganese`.                                        |
| Olivine Vein (GT)    | `Bentonite`, `Magnetite`, `Olivine`, `Glauconite Sand`             | y=-20 to y=10 | `Quartzite`, `Slate`, `Phyllite`, `Schist`, `Gneiss`, `Marble`                | (No specific rock hint)            | GT vein with various industrial minerals.                        |

---

*This detailed mining guide, including the ore reference tables, should provide a strong foundation for resource acquisition in Gravitas². Successful mining requires patience, careful observation, strategic use of tools, and a good understanding of TFC's geology. Always refer to your in-game TFC Guidebook and JEI for the most up-to-date and pack-specific information.*

> Gravitas² | [CurseForge](https://legacy.curseforge.com/minecraft/modpacks/all-the-mods-gravitas2) | [Github](https://github.com/AllTheMods/Gravitas2)
