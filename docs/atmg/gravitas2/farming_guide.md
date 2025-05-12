---
title: Farming in Depth - A Gravitas² Agricultural Guide
description: Comprehensive guide to crops, fruit trees, and bushes in Gravitas²
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
3.  **Hydration:** Plants need water to grow.
    *   Different plants have different **hydration needs** (a percentage range). They can be under-watered or over-watered, both of which can hinder growth or kill the plant.
    *   Farmland hydration decreases the further it is from a water source block. Irrigation (e.g., with `Aqueducts`) can help manage this.
4.  **Nutrients:** While crops do not strictly *require* nutrients to grow, they certainly benefit greatly from them.
    *   There are three main soil nutrients: **Nitrogen (N)**, **Phosphorous (P)**, and **Potassium (K)**.
    *   Each crop has a **favorite nutrient**.
    *   Consuming its favorite nutrient causes a crop to grow faster and **improves the yield** (more food/seeds) at harvest time.
    *   Consuming a nutrient also has the effect of replenishing the *other two* nutrients in the soil around it by a small amount, contributing to a slow nutrient cycling.
5.  **Special Requirements:** Some crops have additional needs:
    *   **Waterlogging:** Some plants (like `Rice` or `Cranberries`) must be grown in waterlogged farmland.
    *   **Support Sticks:** Some climbing plants (like `Green Beans` or `Tomatoes`) require a `Stick` placed in the farmland block (or an adjacent support structure like a trellis if available) to grow to their full height.
    *   **Spreading:** Some plants (like `Pumpkins` or `Melons`) are spreading crops and will place their fruit on adjacent blocks.

---

## Field Crops Reference

The following table details common field crops found in TFC, along with their essential growing conditions.

| Crop             | Temp. Range (°C) | Hydration Range (%) | Nutrient | Special Notes                                                                |
|------------------|------------------|---------------------|----------|------------------------------------------------------------------------------|
| Barley           | -8 to 26         | 18 - 75             | Nitrogen | Single block crop. Produces `Barley` and `Barley Seeds`.                       |
| Oat              | 3 to 40          | 35 - 100            | Phosphorus | Single block crop. Produces `Oat` and `Oat Seeds`.                             |
| Rye              | -11 to 30        | 25 - 85             | Phosphorus | Single block crop. Produces `Rye` and `Rye Seeds`.                             |
| Maize (Corn)     | 13 to 40         | 75 - 100            | Phosphorus | Two blocks tall. Produces `Maize` and `Maize Seeds`.                           |
| Wheat            | -4 to 35         | 25 - 100            | Phosphorus | Single block crop. Produces `Wheat` and `Wheat Seeds`.                         |
| Rice             | 15 to 30         | 25 - 100            | Phosphorus | Single block crop. **Must be planted on farmland in freshwater one block deep (waterlogged).** Produces `Rice` and `Rice Seeds`. |
| Beet             | -5 to 20         | 18 - 85             | Potassium| Single block crop. Produces `Beet` and `Beet Seeds`.                             |
| Cabbage          | -10 to 27        | 15 - 65             | Nitrogen | Single block crop. Produces `Cabbage` and `Cabbage Seeds`.                       |
| Carrot           | 3 to 30          | 25 - 100            | Potassium| Single block crop. Produces `Carrot` and `Carrot Seeds`.                         |
| Garlic           | -20 to 18        | 15 - 75             | Nitrogen | Single block crop. Produces `Garlic` and `Garlic Seeds`.                         |
| Green Beans      | 2 to 35          | 38 - 100            | Nitrogen | Climbing, two blocks tall. **Requires a `Stick` in the farmland to fully grow.** Produces `Green Beans` and `Green Bean Seeds`. |
| Potatoes         | -1 to 37         | 50 - 100            | Potassium| Single block crop. Produces `Potatoes` and `Potato Seeds`.                       |
| Pumpkins         | 0 to 30          | 30 - 80             | Phosphorus | Spreading crop. Places up to two `Pumpkin Blocks` next to it when mature. Can regrow pumpkins. |
| Melons           | 5 to 37          | 75 - 100            | Phosphorus | Spreading crop. Places up to two `Melon Blocks` next to it when mature. Can regrow melons.   |
| Red Bell Peppers | 16 to 30         | 25 - 60             | Potassium| Pickable crop. Harvest with ++rbutton++ near maturity for `Green Bell Peppers`. Allows regrowth. |
| Yellow Bell Peppers| 16 to 30         | 25 - 60             | Potassium| Pickable crop. Harvest with ++rbutton++ near maturity for `Green Bell Peppers`. Allows regrowth. |
| Onions           | 0 to 30          | 25 - 90             | Nitrogen | Single block crop. Produces `Onions` and `Onion Seeds`.                          |
| Soybean          | 8 to 30          | 40 - 100            | Nitrogen | Single block crop. Produces `Soybean` and `Soybean Seeds`.                       |
| Squash           | 5 to 33          | 23 - 95             | Potassium| Single block crop. Produces `Squash` and `Squash Seeds`.                         |
| Sugarcane        | 12 to 38         | 40 - 100            | Potassium| Two blocks tall. Produces `Sugarcane` and `Sugarcane Seeds`. Used for `Sugar`.     |
| Tomatoes         | 0 to 36          | 30 - 95             | Potassium| Climbing, two blocks tall. **Requires a `Stick` in the farmland to fully grow.** Produces `Tomatoes` and `Tomato Seeds`. |
| Jute             | 5 to 37          | 25 - 100            | Potassium| Two blocks tall. Produces `Jute` (fiber) and `Jute Seeds`.                     |
| Papyrus          | 19 to 37         | 70 - 100            | Potassium| Two blocks tall. Produces `Papyrus` (for paper) and `Papyrus Seeds`.             |

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

    ![Fruit Tree Fruiting Calendar](../img/gravitas2/fruit_tree_calendar.png) <!-- Placeholder for your calendar image -->

### Tall Bushes

Tall bushes are fruit blocks that can grow and spread in all directions, either directly upwards (up to three blocks high) or by placing "canes" on their sides which can mature into new full bush blocks. After a while, bushes stop spreading and reach maturity.

*   **Spreading:** Canes need a solid block under them to take root. A flat, open area free of grass/debris is best.
*   **Hydration:** Unlike fruit trees (which primarily care about rainfall), tall bushes take into account surrounding water blocks to determine their hydration.
*   **Harvesting:** Any full bush block can grow berries, harvestable with ++rbutton++. Harvesting these bushes with a sharp tool (like a `Knife`) has a chance to drop a new bush for replanting. Fully mature bushes will always drop themselves.

#### Tall Bush Reference

| Tall Bush        | Temp. Range (°C) | Rainfall (mm) | Growing Months (Approx.) | Flowering Months (Approx.) | Fruiting Months (Approx.) | Found In                 |
|------------------|------------------|---------------|--------------------------|----------------------------|---------------------------|--------------------------|
| Blackberry Bush  | 7 - 24           | 24 - 100      | Feb - May                | Jun - Jul                  | Aug                       | Areas with few trees   |
| Blueberry Bush   | 7 - 29           | 12 - 100      | Feb - May                | Jun - Jul                  | Aug                       | Areas with few trees   |
| Elderberry Bush  | 10 - 33          | 12 - 100      | Feb - May                | Jun - Jul                  | Aug                       | Areas with few trees   |
| Raspberry Bush   | 5 - 25           | 24 - 100      | Apr - Jul                | Aug - Sep                  | Oct                       | Areas with few trees   |

### Small Bushes

Small bushes are low-lying fruit blocks that typically spawn in forests. They can occasionally spread to surrounding blocks if there isn't too much competition. They go through three visual sizes, and when fully grown, their fruit is harvested with ++rbutton++.

#### Small Bush Reference

| Small Bush            | Temp. Range (°C) | Hydration Range (%) | Growing Months (Approx.) | Flowering Months (Approx.) | Fruiting Months (Approx.) | Found In | Special Notes             |
|-----------------------|------------------|---------------------|--------------------------|----------------------------|---------------------------|----------|---------------------------|
| Bunchberry Bush       | 15 - 35          | 24 - 100            | May - Jul                | Aug - Sep                  | Oct                       | Forests  |                           |
| Cloudberry Bush       | -2 - 17          | 9 - 100             | Feb - May                | Jun - Aug                  | Sep                       | Forests  |                           |
| Cranberry Bush        | -5 - 17          | 30 - 100            | Mar - Jun                | Jul - Aug                  | Sep                       | Forests  | **Grown underwater.**     |
| Gooseberry Bush       | 5 - 27           | 24 - 100            | Apr - Jul                | Aug - Sep                  | Oct                       | Forests  |                           |
| Snowberry Bush        | -7 - 18          | 24 - 100            | Mar - Jun                | Jul - Aug                  | Sep                       | Forests  |                           |
| Strawberry Bush       | 5 - 28           | 12 - 100            | Oct - Dec                | Jan - Feb                  | Mar                       | Forests  |                           |
| Wintergreen Berry Bush| -6 - 17          | 12 - 100            | May - Sep                | Oct - Nov                  | Dec                       | Forests  |                           |
*Berry Bush Fruiting Calendar (General Guide):*

    ![Berry Bush Fruiting Calendar](../img/gravitas2/berry_bush_calendar.png) <!-- Placeholder for your calendar image -->

---

*This guide provides a foundation for TFC agriculture. Successful farming requires careful observation of your environment, understanding plant needs, and adapting your strategies to the seasons. Always consult your in-game TFC Guidebook and JEI for the most precise information relevant to Gravitas².*
