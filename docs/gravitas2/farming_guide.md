---
title: Farming in Depth - Agricultural Guide
description: Comprehensive guide to crops, fruit trees, bushes, fertilizers, beekeeping, and greenhouses in Gravitas²
authors:
 - Xannaeh
---

## Introduction to TFC Agriculture

Farming in TerraFirmaCraft (TFC), and by extension Gravitas², is a detailed and rewarding system, moving beyond simple vanilla mechanics. Successfully cultivating crops and fruit-bearing plants requires understanding their specific needs regarding temperature, hydration, soil nutrients, and seasonality. This guide will provide an in-depth look at these systems to help you establish a thriving agricultural base.

---

## Basic Farming Principles

### Obtaining Seeds & Tools

*   **Seeds:** To start growing crops, you'll first need `Seeds`. These are primarily obtained by finding and breaking **Wild Crops** scattered throughout the world.
    *   When a fully mature domesticated crop dies (either due to weather, old age, or being left to rot), it will often go to seed, dropping more seeds for future planting.
    *   Seeds are also useful as `Bait` for some traps or fishing.
*   **Hoe:** A `Hoe` is essential for preparing farmland. A `Stone Hoe` can be knapped from `Pebbles` and a `Stick` in the early game.
    *   Hoes function similarly to vanilla: ++rbutton++ on `Dirt` or `Grass` blocks to turn them into `Farmland`.
    *   They can also be used to convert `Rooted Dirt` (often found under trees) back into regular `Dirt`.

### Growing Conditions

1.  **Farmland:** All standard crops need to be planted on tilled `Farmland`.
2.  **Temperature:** Each crop has an optimal **temperature range** for growth. If the ambient temperature is too hot or too cold, the plant may grow slowly, fail to mature, or die.
    *   Check individual crop entries (or the TFC Guidebook) for specific temperature needs.
    *   Temperature is influenced by season, time of day, Y-level, and the overall climate of the region.
3.  **Hydration (Keeping Hydrated):** Plants need water to grow.
    *   **Checking Hydration:** To see the hydration of any specific farmland block or crop, you must have a `Hoe` in hand and look at the block. A tooltip will show the current hydration as a percentage from 0% to 100%.
    *   **Factors:** Based on the **Rainfall** in the area, the ground may have some latent moisture. However, this may not be enough, especially for water-intensive crops.
    *   Different plants have different **hydration needs** (a percentage range). They can be under-watered or over-watered, both of which can hinder growth or kill the plant.
    *   **Managing Hydration:** Hydration cannot be directly decreased (except by moving to an area with less rainfall). However, it can be **increased by proximity to nearby water blocks**, much like vanilla farmland (within 4 blocks). Irrigation (e.g., with `Aqueducts`) can also help manage this by bringing water closer to your fields.
4.  **Nutrients:** While crops do not strictly *require* nutrients to grow, they certainly benefit greatly from them.
    *   There are three main soil nutrients: **Nitrogen (N)**, **Phosphorous (P)**, and **Potassium (K)**.
    *   Each crop has a **favorite nutrient**.
    *   Consuming its favorite nutrient causes a crop to grow faster and **improves the yield** (more food/seeds) at harvest time. That means crops that consumed more nutrients drop more food when broken.
    *   Consuming a nutrient also has the effect of replenishing the *other two* nutrients in the soil around it by a small amount, contributing to a slow nutrient cycling.
5.  **Special Requirements:** Some crops have additional needs:
    *   **Waterlogging:** Some plants (like `Rice` or `Cranberries`) must be grown in waterlogged farmland.
    *   **Support Sticks:** Some climbing plants (like `Green Beans` or `Tomatoes`) require a `Stick` placed in the farmland block (or an adjacent support structure like a trellis) to grow to their full height.
    *   **Spreading:** Some plants (like `Pumpkins` or `Melons`) are spreading crops and will place their fruit on adjacent blocks.

---
## Fertilizers: Enhancing Your Soil

Fertilizers are used to add nutrients (`Nitrogen`, `Phosphorous`, `Potassium`) to your farmland, improving crop growth speed and yield.

*   **Application:** To use a fertilizer, hold it in your hand and ++rbutton++ on `Farmland` or directly on a `Crop`. Particles should appear, indicating the fertilizer was successfully added.

### Common Fertilizer Types

| Fertilizer      | N | P | K | Source / Notes                                                               |
|-----------------|---|---|---|------------------------------------------------------------------------------|
| `Compost`       | 40| 20| 40| Product of the `Composter`.           |
| `Bone Meal`     | 0 | 10| 0 | Made from crushed `Bones`.                                                   |
| `Saltpeter`     | 10| 0 | 40| Made from `Saltpeter Ore`.                                                   |
| `Guano`         | 80| 50| 10| Found deep underground and on gravelly shores. Potent fertilizer. |
| `Wood Ash`      | 0 | 10| 30| Produced by breaking `Firepits`. Throwing a `Torch` into water also has a chance. |
| `Sylvite Powder`| 0 | 0 | 50| Made from `Sylvite Ore`. Excellent source of Potassium.                      |

---

## Field Crops Reference

The following table details common field crops found in TFC, along with their essential growing conditions.


=== "Sorted By Hydration Range"

    | Crop             | Temp. Range (°C) | Hydration Range (%) | Nutrient | Special Notes                                                                |
    |------------------|------------------|---------------------|----------|------------------------------------------------------------------------------|
    | Maize (Corn)     | 13 to 40         | **75 - 100**        | Phosphorus | Two blocks tall. Produces `Maize` and `Maize Seeds`.                           |
    | Melons           | 5 to 37          | **75 - 100**        | Phosphorus | Spreading crop. Places up to two `Melon Blocks` next to it when mature. Can regrow melons.   |
    | Papyrus          | 19 to 37         | **70 - 100**        | Potassium| Two blocks tall. Produces `Papyrus` (for paper) and `Papyrus Seeds`.             |
    | Potatoes         | -1 to 37         | **50 - 100**        | Potassium| Single block crop. Produces `Potatoes` and `Potato Seeds`.                       |
    | Soybean          | 8 to 30          | **40 - 100**        | Nitrogen | Single block crop. Produces `Soybean` and `Soybean Seeds`.                       |
    | Sugarcane        | 12 to 38         | **40 - 100**        | Potassium| Two blocks tall. Produces `Sugarcane` and `Sugarcane Seeds`. Used for `Sugar`.     |
    | Green Beans      | 2 to 35          | **38 - 100**        | Nitrogen | Climbing, two blocks tall. **Requires a `Stick` in the farmland to fully grow.** Produces `Green Beans` and `Green Bean Seeds`. |
    | Oat              | 3 to 40          | **35 - 100**        | Phosphorus | Single block crop. Produces `Oat` and `Oat Seeds`.                             |
    | Pumpkins         | 0 to 30          | **30 - 80**         | Phosphorus | Spreading crop. Places up to two `Pumpkin Blocks` next to it when mature. Can regrow pumpkins. |
    | Tomatoes         | 0 to 36          | **30 - 95**         | Potassium| Climbing, two blocks tall. **Requires a `Stick` in the farmland to fully grow.** Produces `Tomatoes` and `Tomato Seeds`. |
    | Rye              | -11 to 30        | **25 - 85**         | Phosphorus | Single block crop. Produces `Rye` and `Rye Seeds`.                             |
    | Wheat            | -4 to 35         | **25 - 100**        | Phosphorus | Single block crop. Produces `Wheat` and `Wheat Seeds`.                         |
    | Rice             | 15 to 30         | **25 - 100**        | Phosphorus | Single block crop. **Must be planted on farmland in freshwater one block deep (waterlogged).** Produces `Rice` and `Rice Seeds`. |
    | Carrot           | 3 to 30          | **25 - 100**        | Potassium| Single block crop. Produces `Carrot` and `Carrot Seeds`.                         |
    | Red Bell Peppers | 16 to 30         | **25 - 60**         | Potassium| Pickable crop. Harvest with ++rbutton++ near maturity for `Green Bell Peppers`. Allows regrowth. |
    | Yellow Bell Peppers| 16 to 30         | **25 - 60**         | Potassium| Pickable crop. Harvest with ++rbutton++ near maturity for `Green Bell Peppers`. Allows regrowth. |
    | Onions           | 0 to 30          | **25 - 90**         | Nitrogen | Single block crop. Produces `Onions` and `Onion Seeds`.                          |
    | Jute             | 5 to 37          | **25 - 100**        | Potassium| Two blocks tall. Produces `Jute` (fiber) and `Jute Seeds`.                     |
    | Squash           | 5 to 33          | **23 - 95**         | Potassium| Single block crop. Produces `Squash` and `Squash Seeds`.                         |
    | Barley           | -8 to 26         | **18 - 75**         | Nitrogen | Single block crop. Produces `Barley` and `Barley Seeds`.                       |
    | Beet             | -5 to 20         | **18 - 85**         | Potassium| Single block crop. Produces `Beet` and `Beet Seeds`.                             |
    | Cabbage          | -10 to 27        | **15 - 65**         | Nitrogen | Single block crop. Produces `Cabbage` and `Cabbage Seeds`.                       |
    | Garlic           | -20 to 18        | **15 - 75**         | Nitrogen | Single block crop. Produces `Garlic` and `Garlic Seeds`.                         |


=== "Sorted By Temperature Range"

    | Crop                | Temp. Range (°C) | Hydration Range (%) | Nutrient   | Special Notes                                                                              |
    |---------------------|------------------|---------------------|------------|--------------------------------------------------------------------------------------------|
    | Garlic              | **-20** to 18    | **15 - 75**         | Nitrogen   | Single block crop. Produces `Garlic` and `Garlic Seeds`.                                       |
    | Rye                 | **-11** to 30    | **25 - 85**         | Phosphorus | Single block crop. Produces `Rye` and `Rye Seeds`.                                           |
    | Cabbage             | **-10** to 27    | **15 - 65**         | Nitrogen   | Single block crop. Produces `Cabbage` and `Cabbage Seeds`.                                     |
    | Barley              | **-8** to 26     | **18 - 75**         | Nitrogen   | Single block crop. Produces `Barley` and `Barley Seeds`.                                     |
    | Beet                | **-5** to 20     | **18 - 85**         | Potassium  | Single block crop. Produces `Beet` and `Beet Seeds`.                                           |
    | Wheat               | **-4** to 35     | **25 - 100**        | Phosphorus | Single block crop. Produces `Wheat` and `Wheat Seeds`.                                       |
    | Potatoes            | **-1** to 37     | **50 - 100**        | Potassium  | Single block crop. Produces `Potatoes` and `Potato Seeds`.                                     |
    | Pumpkins            | **0** to 30      | **30 - 80**         | Phosphorus | Spreading crop. Places up to two `Pumpkin Blocks` next to it when mature. Can regrow pumpkins. |
    | Tomatoes            | **0** to 36      | **30 - 95**         | Potassium  | Climbing, two blocks tall. **Requires a `Stick` in the farmland to fully grow.** Produces `Tomatoes` and `Tomato Seeds`. |
    | Onions              | **0** to 30      | **25 - 90**         | Nitrogen   | Single block crop. Produces `Onions` and `Onion Seeds`.                                        |
    | Green Beans         | **2** to 35      | **38 - 100**        | Nitrogen   | Climbing, two blocks tall. **Requires a `Stick` in the farmland to fully grow.** Produces `Green Beans` and `Green Bean Seeds`. |
    | Oat                 | **3** to 40      | **35 - 100**        | Phosphorus | Single block crop. Produces `Oat` and `Oat Seeds`.                                           |
    | Carrot              | **3** to 30      | **25 - 100**        | Potassium  | Single block crop. Produces `Carrot` and `Carrot Seeds`.                                       |
    | Melons              | **5** to 37      | **75 - 100**        | Phosphorus | Spreading crop. Places up to two `Melon Blocks` next to it when mature. Can regrow melons.  |
    | Jute                | **5** to 37      | **25 - 100**        | Potassium  | Two blocks tall. Produces `Jute` (fiber) and `Jute Seeds`.                                   |
    | Squash              | **5** to 33      | **23 - 95**         | Potassium  | Single block crop. Produces `Squash` and `Squash Seeds`.                                       |
    | Soybean             | **8** to 30      | **40 - 100**        | Nitrogen   | Single block crop. Produces `Soybean` and `Soybean Seeds`.                                     |
    | Sugarcane           | **12** to 38     | **40 - 100**        | Potassium  | Two blocks tall. Produces `Sugarcane` and `Sugarcane Seeds`. Used for `Sugar`.                   |
    | Maize (Corn)        | **13** to 40     | **75 - 100**        | Phosphorus | Two blocks tall. Produces `Maize` and `Maize Seeds`.                                         |
    | Rice                | **15** to 30     | **25 - 100**        | Phosphorus | Single block crop. **Must be planted on farmland in freshwater one block deep (waterlogged).** Produces `Rice` and `Rice Seeds`. |
    | Red Bell Peppers    | **16** to 30     | **25 - 60**         | Potassium  | Pickable crop. Harvest with ++rbutton++ near maturity for `Green Bell Peppers`. Allows regrowth. |
    | Yellow Bell Peppers | **16** to 30     | **25 - 60**         | Potassium  | Pickable crop. Harvest with ++rbutton++ near maturity for `Green Bell Peppers`. Allows regrowth. |
    | Papyrus             | **19** to 37     | **70 - 100**        | Potassium  | Two blocks tall. Produces `Papyrus` (for paper) and `Papyrus Seeds`.                           |

---

## Wild Fruits: Trees and Bushes

Many varieties of wild fruits can be found growing in the world, providing food and seeds/saplings for cultivation. Fruits are generally found on three types of plants: **Fruit Trees**, **Tall Bushes**, and **Small Bushes**.

All fruiting plants have a yearly lifecycle: they grow, form flowers, sprout fruit, and then lay dormant (often during colder months). During their cold/dormant season, they may appear brown and lifeless, becoming green and healthy again in spring. Fruit plants can die of old age or due to improper climate conditions.

### Fruit Trees

Fruit trees grow from tiny `Saplings` into large, flowering trees. The branches are their heart and will grow as long as climate conditions are right. Leaves grow on branches and can flower and fruit depending on the season.

*   **Obtaining Saplings:** To get `Saplings` from a wild fruit tree, break the 'elbow' blocks (branch blocks attached to the trunk or other main branches) with an `Axe`. Saplings can also sometimes be found as drops when breaking leaf blocks or placed on these 'elbow' sections if not too high up.
*   **Planting & Growth:** `Saplings` will only start growing if it's not the dormant season for that fruit. The size of the finished tree is loosely determined by how many saplings are in the original sapling block (more saplings = bigger tree).
*   **Splicing:** More saplings can be added to a growing tree through **Splicing**. To splice, ++rbutton++ an existing sapling/young tree with another `Sapling` of the same type while holding a `Knife` in your off-hand.
*   **Harvesting Fruit:** Fruit is harvested by ++rbutton++ a leaf block that is visibly bearing fruit. This gives one fruit and reverts that part of the plant to its growing stage until it flowers and fruits again, or goes dormant.

#### Fruit Tree Reference

| Fruit Tree        | Temp. Range (°C) | Rainfall (mm) | Growing Months (Approx.) | Flowering Months (Approx.) | Fruiting Months (Approx.) | Notes                                                      |
|-------------------|------------------|---------------|--------------------------|----------------------------|---------------------------|------------------------------------------------------------|
| Banana Tree       | 17 - 35          | 280 - 500     | (Varies by climate)      | (Varies by climate)        | (Varies by climate)       | Grows vertically, lacks leaves, fruits at topmost block. Harvested plant dies, must be replanted. Saplings from flowering part. |
| Cherry Tree       | 5 - 25           | 100 - 350     | Jan - Mar                | Apr - May                  | Jun                       |                                                            |
| Green Apple Tree  | 1 - 25           | 110 - 280     | Mar - Jul                | Aug - Sep                  | Oct                       |                                                            |
| Lemon Tree        | 10 - 30          | 180 - 470     | Feb - May                | Jun - Jul                  | Aug                       |                                                            |
| Olive Tree        | 5 - 30           | 150 - 500     | Mar - Jul                | Aug - Sep                  | Oct                       | Olives can produce `Olive Oil` (fuel for lamps).         |
| Orange Tree       | 15 - 36          | 250 - 500     | Mar - Jun                | Jul - Aug                  | Sep                       |                                                            |
| Peach Tree        | 4 - 27           | 60 - 230      | Dec - Mar                | Apr - May                  | Jun                       |                                                            |
| Plum Tree         | 15 - 31          | 250 - 400     | Jan - Apr                | May - Jun                  | Jul                       |                                                            |
| Red Apple Tree    | 1 - 25           | 100 - 280     | Mar - Jul                | Aug - Sep                  | Oct                       |                                                            |

*Fruiting Calendar (General Guide - specific timings can vary):*

*   **Dormant:** Brown/Lifeless appearance, typically colder months.
*   **Healthy:** Green, growing leaves, often Spring/early Summer.
*   **Flowering:** Visible flowers, mid-to-late Summer/early Autumn.
*   **Fruiting:** Visible fruit, late Summer/Autumn.

---

### Tall Bushes (TFC)

Tall bushes are fruit blocks that can grow and spread in all directions, either directly upwards (up to three blocks high) or by placing "canes" on their sides which can mature into new full bush blocks. After a while, bushes stop spreading and reach maturity.

*   **Spreading:** Canes need a solid block under them to take root. A flat, open area free of grass/debris is best.
*   **Hydration:** Unlike fruit trees (which primarily care about rainfall), tall bushes take into account surrounding water blocks to determine their hydration for spreading and growth.
*   **Harvesting:** Any full bush block can grow berries, harvestable with ++rbutton++. Harvesting these bushes with a sharp tool (like a `Knife`) has a chance to drop a new bush for replanting. Fully mature bushes will always drop themselves when broken.

#### Tall Bush Reference

| Tall Bush        | Temp. Range (°C) | Rainfall (mm) | Growing Months (Approx.) | Flowering Months (Approx.) | Fruiting Months (Approx.) | Found In                 |
|------------------|------------------|---------------|--------------------------|----------------------------|---------------------------|--------------------------|
| Blackberry Bush  | 7 - 24           | 24 - 100      | Feb - May                | Jun - Jul                  | Aug                       | Areas with few trees   |
| Blueberry Bush   | 7 - 29           | 12 - 100      | Feb - May                | Jun - Jul                  | Aug                       | Areas with few trees   |
| Elderberry Bush  | 10 - 33          | 12 - 100      | Feb - May                | Jun - Jul                  | Aug                       | Areas with few trees   |
| Raspberry Bush   | 5 - 25           | 24 - 100      | Apr - Jul                | Aug - Sep                  | Oct                       | Areas with few trees   |

---
### Small Bushes & Other Berry Producers (TFC & Firmalife)

This section covers the standard TFC small, low-lying berry bushes typically found in forests, as well as additional berry and fruit-producing bushes introduced by Firmalife which don't fit the "Tall Bush" spreading mechanic.

*   **TFC Small Bushes:** These are low-lying fruit blocks that typically spawn in forests. They can occasionally spread to surrounding blocks if there isn't too much competition from other bushes. They go through three visual sizes, and when fully grown, their fruit is harvested with ++rbutton++.
*   **Firmalife Bushes:** These may have specific environmental requirements or unique properties.

#### Small Bush & Berry Producer Reference

| Bush Name             | Temp. Range (°C) | Hydration/Rainfall              | Growing Months (Approx.) | Flowering Months (Approx.) | Fruiting Months (Approx.)         | Special Notes & Uses                                     |
|-----------------------|------------------|---------------------------------|--------------------------|----------------------------|------------|----------------------------------------------------------|
| Bunchberry Bush (TFC) | 15 - 35          | Hydration: 24 - 100%            | May - Jul                | Aug - Sep                  | Oct                     | TFC Small Bush type.                                     |
| Cloudberry Bush (TFC) | -2 - 17          | Hydration: 9 - 100%             | Feb - May                | Jun - Aug                  | Sep                    | TFC Small Bush type.                                     |
| Cranberry Bush (TFC)  | -5 - 17          | Hydration: 30 - 100%            | Mar - Jun                | Jul - Aug                  | Sep                     | TFC Small Bush type. **Grown underwater (waterlogged farmland).** |
| Gooseberry Bush (TFC) | 5 - 27           | Hydration: 24 - 100%            | Apr - Jul                | Aug - Sep                  | Oct                           | TFC Small Bush type.                                     |
| Snowberry Bush (TFC)  | -7 - 18          | Hydration: 24 - 100%            | Mar - Jun                | Jul - Aug                  | Sep                        | TFC Small Bush type.                                     |
| Strawberry Bush (TFC) | 5 - 28           | Hydration: 12 - 100%            | Oct - Dec                | Jan - Feb                  | Mar                      | TFC Small Bush type.                                     |
| Wintergreen Berry (TFC)| -6 - 17          | Hydration: 12 - 100%            | May - Sep                | Oct - Nov                  | Dec                      | TFC Small Bush type.                                     |
| Nightshade Berry (Firmalife)| 7 - 24     | Rainfall: 200 - 400mm         | (Varies by climate)      | (Varies by climate)        | (Varies by climate)      | Firmalife. **Poisonous.** Makes `Stinky Soup`.         |
| Pineapple Bush (Firmalife)| 20 - 32    | Rainfall: 250 - 500mm         | (Varies by climate)      | (Varies by climate)        | (Varies by climate)      | Firmalife. Can be processed into `Pineapple Leather` (Dry -> Fiber -> Yarn -> Leather).      |



---

## Beekeeping In-Depth

Bees are incredibly useful for pollinating your crops, providing food (`Honey`), and essential crafting materials like `Beeswax` (for `Treated Lumber`, vital for Create mod progression).

### 1. Setting Up Your Apiary

*   **Craft `Beehive Frames`:** Essential components.
*   **Craft `Wooden Beehive`:** Requires `Beehive Frames` and `Lumber`.
*   **Placement:** Place your `Wooden Beehive`. Beehives can share flowers if placed relatively close (within their 5-block radius check for flowers). The benefit of flowers diminishes after around 60 flowers for a single hive.

### 2. Attracting and Housing Bees

*   **Frames are Key:** Bees need `Beehive Frames` inside the hive to live. Having **4 empty `Beehive Frames`** in a hive greatly increases the chances of a wild swarm moving in.
*   **Flower Power:** A hive needs at least **10 `Flowers`** planted within a 5-block radius for a chance for an empty frame to be populated with a `Queen Bee`. More flowers can help. Bee particles around the hive indicate this colonization attempt.
*   **Patience & Queens:** Wild swarms may take time to colonize. If you find a `Queen Bee` item, placing it in a frame within the hive can significantly speed this up.

### 3. Harvesting Resources Safely

*   **WARNING: DO NOT INTERACT WITH ACTIVE BEEHIVES DURING DAYTIME** (unless smoked). Bees will attack if you disturb them (e.g., by removing frames).
*   **Safe Harvesting:**
    *   **Night:** Interact with hives at night when bees are sleeping.
    *   **Smoke:** An active `Firepit` (burning `Logs`) placed directly underneath the `Beehive` can pacify the bees for daytime harvesting.
*   **`Honey`:** When a hive visibly has honey, ++rbutton++ the hive with an `Empty Jar` to collect a `Honey Jar`. Opening the `Honey Jar` (e.g., in a crafting grid) gives `Raw Honey`, a sugar substitute.
*   **`Beeswax`:**
    *   When a frame is filled with honeycomb, remove it (safely).
    *   ++rbutton++ the filled frame in your inventory with a `Knife` to get `Beeswax`.
    *   **Critical: This process kills the queen in that frame!** Be mindful, especially early on. Ensure you have other queens or methods to attract new ones.
*   **`Treated Lumber`:** The most important early use of `Beeswax` is crafting `Treated Lumber`. This is vital for Create mod progression.

### 4. Bee Abilities and Breeding (Advanced)

*   **Breeding:** If a beehive has two frames with queens and an empty frame, the colonies may breed, producing a new queen in the empty frame. This passes on **Abilities** (traits) from the parents. Abilities are on a scale of 1-10.
*   **List of Abilities:**
    *   **Hardiness:** Allows honey production at lower temperatures (Hardiness 10: down to -16°C; Hardiness 1: down to 2°C).
    *   **Production:** Improves honey production speed.
    *   **Mutant:** Increases variability in traits passed during breeding.
    *   **Fertility:** Increases likelihood of breeding.
    *   **Crop Affinity:** Likelihood of spreading a small amount of nutrients to nearby crops.
    *   **Nature Restoration:** Causes new flowers and lilypads to spawn around the hive.
    *   **Calmness:** Decreases likelihood of bees attacking you.
*   **Genetic Disease:** Bees with high Mutant ability have a chance of developing a Genetic Disease. Diseased bees pass it to offspring and don't produce honey.

### 5. Bee Tips

*   Bees can help fertilize planters and crops via Crop Affinity.
*   Scraping a frame for beeswax sacrifices that queen. Be smart!
*   Being wet (e.g., in water) prevents bees from attacking you.

---
## Greenhouses: Year-Round Cultivation

The `Greenhouse` is a multiblock device controlled by a `Climate Station`. It allows growing crops year-round, bypassing seasonal restrictions. Building a greenhouse is quite simple, but requires adherence to specific rules.

### Building Your Greenhouse

Constructing a functional greenhouse involves creating an enclosed space using specific greenhouse blocks:

1.  **Enclosed Structure:** The greenhouse must be a fully enclosed area of blocks, similar to a `Cellar`.
2.  **Walls:**
    *   The walls of greenhouses must be **solid faces**.
    *   If using **Panel Walls**, they should be placed so that the face that is on the exterior of the block (e.g., the face you can place a torch on) faces *into* the greenhouse.
3.  **Roof:**
    *   The same orientation rule applies to panel roofs as panel walls.
    *   `Slabs` are always considered valid roof blocks, regardless of their orientation.
4.  **Doors & Trapdoors:** Standard greenhouse `Doors` and `Trapdoors` are always valid and require no special placement.
5.  **Floor:** The floor of the greenhouse may be any non-air block; it does not need to be a specific greenhouse block.
6.  **Homogeneous Type:** All greenhouse blocks used in the structure (walls, roof, doors, etc.) must belong to the *same* **Greenhouse Type** (e.g., all Treated Wood, or all Copper).

### Greenhouse Types

Greenhouse Types are families of greenhouse blocks that can be used interchangeably in a greenhouse. Most greenhouse blocks age. For example, `Treated Wood` greenhouse blocks become `Weathered Treated Wood` blocks. Since both of these block types belong to the same greenhouse type, your greenhouse will continue to function.

These are the Greenhouse Types available, with the block types they can age into:

*   **Treated Wood:** Weathered
*   **Copper:** Exposed, Weathered, Oxidized
*   **Iron:** Rusted
*   **Aluminium:** (Does not age)

*Initially, only Treated Wood greenhouses might be available. Copper, Iron, and Aluminium represent tiers of advancement, often required for specific advanced crops or planters.*

### Greenhouse Blocks & Components

There are four types of regular `Greenhouse Blocks`: Walls, Doors, Roofs, and Roof Tops. Roofs and Roof Tops are stairs and slabs, respectively. There are also thinner versions of these blocks, also known as panel walls, trapdoors, and panel roofs. These can be combined however you choose to form the structure of the greenhouse.

*   **Regular Blocks:**
    *   `Greenhouse Wall`
    *   `Greenhouse Door`
    *   `Greenhouse Roof` (Stairs)
    *   `Greenhouse Roof Top` (Slabs)
*   **Panel Blocks (Thinner Variants):**
    *   `Greenhouse Panel Wall`
    *   `Greenhouse Trapdoor`
    *   `Greenhouse Panel Roof`
*   **Specialized Blocks:**
    *   `Greenhouse Port`: A wall block with an integrated pipe segment, allowing `Copper Pipes` to pass water through the greenhouse wall without breaking the seal.

### Greenhouse Operations & Internal Devices

There are many blocks that operate inside Greenhouses:

*   **`Climate Station`:** The control block for the greenhouse. It must be placed within or connected to the greenhouse structure to activate it.
*   **`Planters`:** For growing crops.
*   **`Sprinklers`:** Various devices that add water to planters.

### Greenhouse Irrigation System

To automate watering within your greenhouse, you'll typically use a system of sprinklers, pipes, and a water source.

*   **`Sprinkler`:**
    *   **Function:** The `Sprinkler` is a device that sprinkles water in a 5x6x5 area centered on the block *below* the sprinkler block. You know it is working when it drips out water particles. Sprinklers placed facing up irrigate the same 5x6x5 area *above*.
*   **`Copper Pipe`:**
    *   **Function:** Sprinklers must be connected to a system of pipes that feed it water in order to work. This is done by connecting a series of `Copper Pipes` to them. `Copper Pipes` transport water up to 32 blocks to a sprinkler. They are connected to `Irrigation Tanks` or `Pumping Stations`.
*   **`Pumping Station`:**
    *   **Function:** `Pumping stations` must be above a source block of water in order to work, and be connected to mechanical power.
*   **`Irrigation Tank`:**
    *   **Function:** `Irrigation tanks` can also serve water through their ports on the sides, provided that they are stacked at most 3 blocks high above a pumping station or on other tanks.
*   **`Oxidized Copper Pipe`:**
    *   **Function:** Oxidized pipes are the same as regular copper pipes, except they do not connect to the other kind of pipe.

### Planters: The Heart of Greenhouse Farming

`Planters` are used to grow crops inside a `Greenhouse`. To see the status of a planter, you can look at it while holding a `Hoe`. Crops in planters consume `Nutrients` in a similar way to `Crops`. Planters should be placed inside a valid Greenhouse and activated with a `Climate Station`. Planters need at least some natural sunlight to work.

*   **Watering:** Planters must be Watered to grow. This is done with a `Watering Can`, or automatically with `Sprinklers`.
*   **`Watering Can`:**
    *   **Use:** Press ++rbutton++ with it to water nearby planters. Refill it by pressing ++rbutton++ on a water source.

#### Types of Planters and Their Crops

Different planters are suited for different types of crops and may have specific greenhouse tier requirements.

*   **`Large Planter`**
    *   **Grows:** Single crop from seed. Large Planters can grow Green Beans, Tomatoes, Sugarcane, Jute, and Grains.
    *   **Harvest:** Harvested with ++rbutton++ when mature.
    *   **Requirements:** To grow Grains (e.g., Wheat, Rye, Barley, Rice, Maize, Oats), you need a **Copper or better** greenhouse. Other listed crops can be grown in any greenhouse type.

*   **`Quad Planter`**
    *   **Grows:** Four individual crops at once. Quad Planters can grow Beets, Cabbage, Carrots, Garlic, Onions, Potatoes, and Soybeans.
    *   **Nutrients:** These crops all draw from the same nutrient pool.
    *   **Harvest:** Can be harvested individually with ++rbutton++ when mature.
    *   **Requirements:** These crops can be grown in **any** greenhouse type.

*   **`Bonsai Planter`**
    *   **Grows:** Small fruit trees from their saplings. Bonsai Planters can grow any fruit tree type, *except* Bananas (which need a `Hanging Planter`).
    *   **Nutrient:** They all consume Nitrogen as their main nutrient.
    *   **Harvest:** The fruit can be picked with ++rbutton++.
    *   **Requirements:** Requires an **Iron or better** greenhouse to grow.

*   **`Hanging Planter`**
    *   **Grows:** Crops upside down. Hanging Planters grow Squash (from their seeds) and Bananas (from their saplings).
    *   **Placement:** Need to anchor to a solid block above them.
    *   **Harvest:** When mature, they can be harvested with ++rbutton++.
    *   **Requirements:** Squash can be grown in **any** greenhouse type, but Bananas require an **Iron or better** greenhouse to grow.

*   **`Trellis Planter`**
    *   **Grows:** Berry bushes. Trellis Planters can grow any berry bush *except* Cranberries.
    *   **Mechanic:** Trellis Planters have the unique property of propagating berry bushes. If a trellis planter is placed on top of another, and the one below has a mature berry bush, it has a chance to grow upwards into the next one.
    *   **Nutrient:** Bushes prefer Nitrogen.
    *   **Harvest:** Berries can be picked with ++rbutton++.
    *   **Requirements:** Requires an **Iron or better** greenhouse to work.

*   **`Hydroponic Planter`**
    *   **Grows:** Rice and Cranberry bushes.
    *   **Mechanic:** They work the same as a quad planter, except that they do not need to be watered.
    *   **Watering:** Instead, they *must* have an active irrigation pipe (e.g., `Copper Pipe` connected to a sprinkler system) directly below them that is supplying water. Without the pipe, they will not grow.
    *   **Requirements:** Greenhouse tier not explicitly stated for the planter itself; likely depends on the crop if not for the special watering. Assumed "Any" if water conditions are met.

### Greenhouse Crop Planting Guide

This table summarizes which planters to use for various crops within a greenhouse and any minimum greenhouse tier requirements.

| Crop             | Planter Type        | Min. Greenhouse Level | Notes                                                                 |
|------------------|---------------------|-----------------------|-----------------------------------------------------------------------|
| Wheat            | Large Planter       | Copper                |                                                                       |
| Rye              | Large Planter       | Copper                |                                                                       |
| Barley           | Large Planter       | Copper                |                                                                       |
| Rice             | Hydroponic Planter       | Copper                |                             |
| Maize (Corn)     | Large Planter       | Copper                |                                                                       |
| Oat              | Large Planter       | Copper                |                                                                       |
| Green Beans      | Large Planter       | Any                   |                                                                       |
| Tomatoes         | Large Planter       | Any                   |                                                                       |
| Sugarcane        | Large Planter       | Any                   |                                                                       |
| Jute             | Large Planter       | Any                   | (Fiber crop)                                                          |
| Beets            | Quad Planter        | Any                   |                                                                       |
| Cabbage          | Quad Planter        | Any                   |                                                                       |
| Carrots          | Quad Planter        | Any                   |                                                                       |
| Garlic           | Quad Planter        | Any                   |                                                                       |
| Onions           | Quad Planter        | Any                   |                                                                       |
| Potatoes         | Quad Planter        | Any                   |                                                                       |
| Soybeans         | Quad Planter        | Any                   |                                                                       |
| Squash           | Hanging Planter     | Any                   | Grows upside down.                                                    |
| All (except Banana)| Bonsai Planter      | Iron                  | Saplings. Prefers Nitrogen.                                           |
| Banana           | Hanging Planter     | Iron                  | Saplings. Grows upside down.                                          |
| All (except Cranberry)| Trellis Planter     | Iron                  | Can propagate upwards. Prefers Nitrogen.                            |
| Cranberry        | Hydroponic Planter  | Any (if water met)    | Requires active irrigation pipe below.                                |

*Note: "Any (if water met)" for Hydroponic Planter crops indicates the planter itself doesn't seem to have a tier, but relies on its special watering. The specific crop (e.g. Rice) might have its own needs if grown conventionally.*

---

## Firmalife Specialities: Winemaking

Firmalife introduces winemaking, the science of turning grapes into alcohol. While wine in Firmalife might not have special uses beyond regular TFC alcohol, it's a flavorful addition to your homestead.

### 1. Finding Grapes

*   **`Wild Red Grapes` & `Wild White Grapes`:** Spawn from 0-30°C and 125-500mm rainfall (almost the entire habitable area).

### 2. Growing Grapes: Trellises

Grapes must be grown on **trellises**.

*   **`Grape Trellis Post`:** Craft these first.
*   **Constructing a Trellis:**
    1.  Place two `Grape Trellis Posts` on top of each other.
    2.  Move two blocks to the left or right (so you just need to leave a block in between the trellis) and repeat, placing another stack of two posts.
    3.  ++rbutton++ the side of one of the top and bottom posts with `Jute Fiber` (from `Jute` plants) to string lines between the posts.
    4.  Grape trellises can be chained horizontally to create rows.
*   **Growth:** Provided climate requirements are met, grapes will grow up and over the trellis over a few months, typically fruiting in July after flowering the month prior. Grapes can also be grown in greenhouses.

### 3. Processing Grapes

*   **Harvesting:** Harvest grapes from the trellis when ripe.
*   **Stomping:**
    *   Craft an `Acacia Stomping Barrel` (or other wood type).
    *   ++rbutton++ the Stomping Barrel with fresh grapes to add them.
    *   Jump up and down on the barrel 16 times.
    *   ++rbutton++ with an empty hand to retrieve the result.
    *   A `Quern` may also be used to smash grapes.
*   **Fermenting:** Seal the processed grapes/juice in a `Barrel` for 5 days to ferment them into young wine.
*   **Barrel Press (Optional Aging/Refining):**
    *   Craft an `Acacia Barrel Press` (or other wood type).

### 4. Bottling and Types of Wine

*   **Wine Bottles:** Wine must be bottled in proper `Wine Bottles`, made from non-silica glass.
    *   The TFC Guidebook image shows a glassblowing-like process: 1. Blow, 2. Blow, 3. Pinch, 4. Saw.
*   **Mixing:** The leftmost slot in a bottling interface (perhaps the Barrel Press GUI or a dedicated bottler) can hold up to 16 grape items. Four grape items are needed for one bottle of wine.
    *   Central slots may be for mixing grapes with other ingredients (optional).
    *   Using only red or white grapes yields red or white wine.
    *   Adding at least one red grape to white wine makes Rosé.
    *   Adding `Sugar` to white wine makes dessert wine.
*   **Corks & Labels:**
    *   Wine must be provided with a `Cork`. Corks are made by soaking `Treated Lumber` in `Limewater` for a day.
    *   When all is complete, use the bottle slot to fill the wine, or by ++rbutton++ with a `Wine Bottle` in hand on the aging/bottling device.
    *   **`Bottle Labels`:** Can be crafted (e.g., `Paper`, `Ink`, `String/Cork Piece`). Rename them in a Scribing Station to add their name to the wine's tooltip.

---

*This guide provides a foundation for TFC agriculture. Successful farming requires careful observation of your environment, understanding plant needs, and adapting your strategies to the seasons. Always consult your in-game TFC Guidebook and JEI for the most precise information relevant to Gravitas².*

> TerraFirmCraft | [CurseForge](https://www.curseforge.com/minecraft/mc-mods/terrafirmacraft) | [GitHub](https://github.com/TerraFirmaCraft/TerraFirmaCraft) | [Wiki](https://terrafirmacraft.github.io/Field-Guide/en_us/)
