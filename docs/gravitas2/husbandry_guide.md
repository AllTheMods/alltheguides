---
title: Guide to Animals and Husbandry
description: Understanding wild animals, taming, breeding, and livestock management in TerraFirmaCraft for Gravitas².
authors:
 - Xannaeh
---

## Introduction to Animals in TerraFirmaCraft

The world of TerraFirmaCraft (TFC) is teeming with diverse animal life. Some animals can be beneficial to the player, providing resources or companionship, while others pose significant threats. This guide will cover `Animal Husbandry` for taming, breeding, and managing livestock, as well as details on other `Tameable Wild Animals` and general `Wild Animals`.

---

## Animal Husbandry

`Animal Husbandry` in TFC involves taming, breeding, and managing `Livestock` animals. These animals provide valuable resources and utility.

**Core Husbandry Mechanics:**
*   **Sex:** Livestock can be male or female. Some species have visual distinctions (e.g., male pigs have tusks).
*   **Aging:** Animals progress through life stages:
    *   **Baby:** Smaller, cannot provide resources or breed.
    *   **Adult:** Mature after a set number of days; can breed and produce resources.
    *   **Old:** After extensive use or breeding, animals become old and are primarily useful only for their meat. Old animals may show visual signs like faded coats (e.g., an old bull).
*   **Familiarity:**
    *   Raised by feeding animals their preferred foods (Left Shift + Right Click with food).
    *   Decays daily if not fed. Sufficiently high familiarity (indicated by a white outlined heart icon) prevents decay.
    *   View familiarity by holding Left Shift and looking at the animal.
    *   Adult livestock cannot reach 100% familiarity (red outlined heart); babies can.
*   **Mammals and Pregnancy:**
    *   Adult `Mammals` with >30% familiarity, if fed on a given day, will mate if near an opposite-gendered adult of the same species.
    *   The female becomes `pregnant` and will give birth after a species-specific gestation period.
*   **Wooly Animals:**
    *   `Mammals` that can be `Sheared` for wool when adult and sufficiently familiar. Examples: `Sheep`, `Alpacas`, `Musk Oxen`.
*   **Dairy Animals:**
    *   `Mammals` that produce `Milk`. Adult, familiar females can be milked using a `Bucket`. Examples: `Goats`, `Cows`, `Yaks`.
*   **Oviparous Animals (Egg-Layers):**
    *   Not mammals; reproduce by laying `Eggs`. Examples: `Ducks`, `Quails`, `Chickens`.
    *   Require a `Nest Box` to lay eggs, which they can locate on their own.
        *   **Nest Box Crafting:** 3 `Straw` (top row) + 3 `Lumber` (bottom row).
    *   Male oviparous animals can fertilize females, causing the next egg laid in a nest box to be fertilized.
    *   Fertilized eggs have a tooltip indicating hatch time.
    *   `Eggs` can be cooked or boiled for food.
*   **Equines (Rideable Animals):**
    *   `Mammals` that can be ridden once tamed (reaching 15% familiarity).
    *   Require a `Saddle` to be ridden, which can be `Knapped`.
    *   Includes `Mules`, `Donkeys`, and `Horses`.
    *   `Mules` and `Donkeys` can be equipped with a `Chest` or `Barrel`.
        *   To remove a `Barrel`: Left Shift + Right Click with an empty hand.
        *   To drain fluid from an equipped `Barrel`: Left Shift + Right Click with a `Bucket`.

### Husbandry Animals Table

| Animal    | Biome             | Temp °C      | Rainfall mm | Diet                                              | Primary Products/Use | Breeding Group | Children | Pregnancy / Hatch Time | Max Litters / Eggs | Adulthood | Production Cycle                 | Other Notes                                                      |
|-----------|-------------------|--------------|-------------|---------------------------------------------------|----------------------|----------------|----------|------------------------|--------------------------|-----------|----------------------------------|------------------------------------------------------------------|
| Pig       | Mild forests      | -10 to 35    | ≥ 200       | Any food (even rotten)                            | Meat                 | Mammal         | 1-10     | 19 days                | 6l                       | 80 days   | ---                              | Male pigs have tusks.                                            |
| Cow       | Most climates     | -10 to 35    | ≥ 250       | `Grains` (rotten ok)                              | Milk, Meat           | Mammal         | 1-2      | 58 days                | 13l                      | 192 days  | Milk daily                       | Dairy Animal. Can be milked 128 times if never bred.               |
| Goat      | Moderate climates | -12 to 25    | ≥ 300       | `Grains`, `Fruits`, `Vegetables` (rotten ok)        | Milk, Meat           | Mammal         | 1-2      | 32 days                | 6l                       | 96 days   | Milk every 3 days                | Dairy Animal. Can be milked 60 times if never bred.              |
| Yak       | Cold climates     | ≤ -11        | ≥ 100       | Fresh `Grains` only                               | Milk, Meat           | Mammal         | 1        | 64 days                | 23l                      | 180 days  | Milk daily                       | Dairy Animal. Can be milked 230 times if never bred.             |
| Alpaca    | Moderate climates | -8 to 20     | ≥ 250       | `Grains`, `Fruits`                                | Wool, Meat           | Mammal         | 1-2      | 36 days                | 13l                      | 98 days   | Grows wool every 6 days          | Wooly Animal. Can be sheared 128 times if never bred.            |
| Sheep     | Drier climates    | 0 to 35      | 70-300      | `Grains`                                          | Wool, Meat           | Mammal         | 1-2      | 32 days                | 6l                       | 56 days   | Grows wool every 9 days          | Wooly Animal. Can be sheared 60 times if never bred.             |
| Musk Ox   | Cold climates     | -25 to 0     | ≥ 100       | `Grains`                                          | Wool, Meat           | Mammal         | 1        | 64 days                | 16l                      | 168 days  | Grows wool every 96h (4 days)    | Wooly Animal. Sheared 160 times if never bred.                   |
| Chicken   | Warm forests      | ≥ 14         | ≥ 225       | `Grains`, `Fruits`, `Vegetables`, `Seeds` (rotten ok) | Eggs, Meat           | Oviparous      | 1 (egg)  | 8 days                 | 100 eggs                     | 24 days   | Produces eggs every 30 hours     | Requires Nest Box to lay/fertilize eggs.                         |
| Duck      | Most plains       | -25 to 30    | ≥ 100       | `Grains`, `Fruits`, `Vegetables`, `Bread`, `Seeds`  | Eggs, Meat           | Oviparous      | 1 (egg)  | 8 days                 | 72 eggs                  | 32 days   | Produces eggs every 32 hours     | Requires Nest Box to lay/fertilize eggs.                         |
| Quail     | Colder climates   | -15 to 15    | ≥ 200       | `Grains`, `Fruits`, `Vegetables`, `Seeds` (rotten ok) | Eggs, Meat           | Oviparous      | 1 (egg)  | 8 days                 | 48 eggs                  | 22 days   | Produces eggs every 28 hours     | Requires Nest Box to lay/fertilize eggs.                         |
| Donkey    | Wetter plains     | ≥ -15        | 130-400     | `Grains`, `Fruits`                                | Transport (Chest), Meat | Mammal         | 1        | 19 days                | 6 litters                | 80 days   | ---                              | Equine. Rideable. Can carry a chest/barrel.                      |
| Mule      | Plains            | ≥ -15        | 130-400     | `Grains`, `Fruits`                                | Transport (Chest), Meat | Mammal         | N/A      | N/A                    | N/A (Sterile)            | 80 days   | ---                              | Equine. Rideable. Can carry chest/barrel. Always male. Sterile.  |
| Horse     | Plains            | ≥ -15        | 130-400     | `Grains`, `Fruits`                                | Transport, Meat      | Mammal         | 1        | 19 days                | 6 litters                | 80 days   | ---                              | Equine. Rideable.                                                |

---

## Tameable Wild Animals

Some wild animals, while not part of the formal livestock system, can be tamed by the player for companionship or utility.

| Animal | Spawning Conditions (Biome, Temp °C, Rainfall mm) | Behavior / Key Drops          | Taming Information                                       |
|--------|---------------------------------------------------|-------------------------------|----------------------------------------------------------|
| Wolf   | Any biome; Temp < 22°C; Rainfall 150mm - 420mm    | Hunts in packs                | Tamed into a `Dog` by feeding it multiple times.         |
| Ocelot | Forests; Temp 15°C to 30°C; Rainfall 300mm - 500mm | Attacks small animals         | Tamed into a `Cat` by feeding it raw fish multiple times.|

---

## Other Wild Animals

These animals inhabit the world but are generally not tamed for husbandry or direct companionship.

**General Predator Behavior:** Can actively hunt and attack the player. May be nocturnal (hunt at night) or diurnal (hunt during day). Can be neutral or hostile, often defending a home territory.
**General Ramming Animal Behavior:** Occasionally charge nearby creatures, including the player. Attacks are powerful but can be dodged. Become more aggressive if attacked.
**General Prey Animal Behavior:** Fear players and predators, adept at fleeing. Generally cannot fight back. Some may eat crops.
**Aquatic Animal Categories:**
*   **Shore Animals:** Spawn on sea shores, mix swimming and walking. Curious, may follow player, but not tamable.
*   **Fish:** Swim in water, most can be fished. Prefer various water bodies/temperatures.
*   **Shellfish:** Live on water floors, drop shells (food/flux/bait). Cannot be fished.
*   **Large Water Creatures:** Larger animals in big water bodies. Some hunt fish. Drop `blubber` (lamp fuel).

| Animal        | Category                | Spawning Conditions (Biome, Temp °C, Rainfall mm)                      | Key Behavior / Drops                                                |
|---------------|-------------------------|------------------------------------------------------------------------|---------------------------------------------------------------------|
| Polar Bear    | Predator                | Coldest regions; Temp ≤ -10°C; Rainfall ≥ 100mm                         | Hostile                                                             |
| Grizzly Bear  | Predator                | Forests, moderate climates; Temp -15°C to 15°C; Rainfall ≥ 200mm        | Hostile                                                             |
| Black Bear    | Predator                | Forests, warmer, wetter climates; Temp 5°C to 20°C; Rainfall ≥ 250mm    | Hostile                                                             |
| Cougar        | Predator                | Most moderate climates; Temp -10°C to 21°C; Rainfall ≥ 150mm             | Hostile                                                             |
| Panther       | Predator                | Most moderate climates; Temp -10°C to 21°C; Rainfall ≥ 150mm             | Hostile                                                             |
| Lion          | Predator                | Plains; Avg Temp ≥ 16°C; Rainfall 50mm - 300mm                          | Hostile                                                             |
| Tiger         | Predator                | Forests; Avg Temp ≥ 13°C; Rainfall ≥ 100mm                              | Hostile                                                             |
| Sabertooth    | Predator                | Any biome; Temp > 0°C; Rainfall > 250mm                                 | Hostile                                                             |
| Direwolf      | Predator                | Any biome; Temp < 0°C (below freezing); Rainfall 150mm - 420mm          | Hunts in packs. Larger than regular wolves.                         |
| Hyena         | Predator                | Any biome; Temp > 15°C; Rainfall 80mm - 380mm                           | Hunts in packs.                                                     |
| Crocodile     | Predator                | Near rivers, lakes, marshes; Temp > 15°C; Any rainfall                  | Nocturnal. Most dangerous in water.                                 |
| Boar          | Ramming                 | Any biome; Temp -5°C to 25°C; Rainfall 130mm - 400mm                     | Charges if provoked or nearby. (Pigs are domestic version)        |
| Moose         | Ramming                 | Forests; Temp -15°C to 10°C; Rainfall 150mm - 300mm                      | Charges if provoked or nearby.                                      |
| Wildebeest    | Ramming                 | Open plains; Temp > 13°C; Rainfall 90mm - 380mm                         | Charges if provoked or nearby.                                      |
| Rabbit        | Prey                    | Ubiquitous; Min Rainfall 15mm                                           | Flees, chews on carrots/cabbage. Coat changes by climate.         |
| Fox           | Prey                    | Forests; Temp < 25°C; Rainfall 130mm - 400mm                            | Flees, eats berries from bushes.                                    |
| Deer          | Prey                    | Forests; Temp -15°C to 25°C; Rainfall 130mm - 400mm                      | Flees.                                                              |
| Caribou       | Prey                    | Any biome; Temp < -9°C; Rainfall 110mm - 500mm                          | Flees.                                                              |
| Gazelle       | Prey                    | Open plains; Temp > 12°C; Rainfall 90mm - 380mm                         | Flees.                                                              |
| Bongo         | Prey                    | Forests; Temp > 15°C; Rainfall 230mm - 500mm                            | Flees.                                                              |
| Grouse        | Prey                    | Any biome; Temp -12°C to 13°C; Rainfall 150mm - 400mm                    | Flees.                                                              |
| Pheasant      | Prey                    | Forests; Temp -5°C to 17°C; Rainfall 100mm - 300mm                       | Flees.                                                              |
| Turkey        | Prey                    | Forests; Temp 0°C to 17°C; Rainfall 250mm - 450mm                        | Flees. (Chickens/Ducks/Quails are domestic fowl)                    |
| Peafowl       | Prey                    | Forests; Temp > 14°C; Rainfall 130mm - 500mm                            | Flees.                                                              |
| Penguin       | Aquatic (Shore Animal)  | Coldest beaches; Temp ≤ -14°C; Rainfall ≥ 75mm                           | Curious, follows player.                                            |
| Sea Turtle    | Aquatic (Shore Animal)  | Warm water beaches; Temp ≥ 21°C; Rainfall ≥ 250mm                        | Curious.                                                            |
| Cod           | Aquatic (Fish)          | Colder oceans; Temp ≤ 18°C                                             | Swims, can be fished.                                               |
| Pufferfish    | Aquatic (Fish)          | Any ocean; Temp ≥ 10°C                                                 | Swims.                                                              |
| Jellyfish     | Aquatic (Fish)          | Warmer oceans; Temp ≥ 18°C                                             | Swims.                                                              |
| Tropical Fish | Aquatic (Fish)          | Warmer oceans; Temp ≥ 18°C                                             | Swims.                                                              |
| Salmon        | Aquatic (Fish)          | Any river or lake; Temp ≥ -5°C                                         | Swims.                                                              |
| Bluegill      | Aquatic (Fish)          | Any river or lake; Temp -10°C to 26°C                                  | Swims.                                                              |
| Isopod        | Aquatic (Shellfish)     | Deeper sections of oceans; Temp ≤ 14°C                                 | Drops shells (food/flux/bait).                                      |
| Lobster       | Aquatic (Shellfish)     | Any ocean; Temp ≤ 21°C                                                 | Drops shells (food/flux/bait).                                      |
| Crayfish      | Aquatic (Shellfish)     | Rivers and lakes; Temp ≥ 5°C; Rainfall ≥ 125mm                         | Drops shells (food/flux/bait).                                      |
| Horseshoe Crab| Aquatic (Shellfish)     | Oceans, moderate climate; Temp 10°C to 21°C; Rainfall ≤ 400mm          | Drops shells (food/flux/bait).                                      |
| Orca          | Aquatic (Large Creature)| Deep oceans; Temp ≤ 19°C; Rainfall ≥ 100mm                               | Hunts fish, drops `blubber`.                                        |
| Dolphin       | Aquatic (Large Creature)| Deep oceans; Temp ≥ 10°C; Rainfall ≥ 200mm                               | Drops `blubber`.                                                    |
| Manatee       | Aquatic (Large Creature)| Warm lakes; Temp ≥ 20°C; Rainfall ≤ 300mm                                | Drops `blubber`.                                                    |
| Squid         | Aquatic (Large Creature)| Any deep ocean                                                         | Drops `Ink Sacs`. Inks players. Some say strange properties in deep caves. |

---

*This guide provides an overview of animals and husbandry in Gravitas² based on TerraFirmaCraft mechanics. Always refer to in-game information and specific modpack configurations for the most accurate details.*

> TerraFirmCraft | [CurseForge](https://www.curseforge.com/minecraft/mc-mods/terrafirmacraft) | [GitHub](https://github.com/TerraFirmaCraft/TerraFirmaCraft) | [Wiki](https://terrafirmacraft.github.io/Field-Guide/en_us/)
