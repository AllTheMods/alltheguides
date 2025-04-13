---
title: Curios Guide
description: A Guide for Curios Slots and Items in All the Magic - Arcana (ATMA)
authors:
 - Xannaeh
---

# Guide: Curios Slots & Items

This guide covers the Curios API, how to gain additional slots, and provides details on specific Curios items available in ATMA, with examples from various mods.

## Understanding Curios: The Accessory API

### Overview

**Curios** is a foundational Minecraft mod acting as an **API** (Application Programming Interface) and library. It primarily provides a standardized system for other mods to add **new equipment slots** beyond vanilla armor, off-hand, and hotbar slots. Think of it as a framework enabling accessories and extra gear.

### Key Features for Players:

*   **More Equipment Slots:** Allows mods to add slots for items like rings, necklaces, belts, charms, back items, headgear, hand items, and more.
*   **Centralized Management:** All extra accessory slots are managed through a single GUI, typically opened by pressing the **'G' key** (configurable in Controls). This keeps your main inventory screen cleaner.
*   **Flexibility:** Items can often be equipped into multiple compatible slot types (e.g., some head items might fit in the helmet slot or a Curios head slot).
*   **Compatibility:** Standard mechanics like Mending, Unbreaking, and Curses generally work with items in Curios slots.

![Curios Slots GUI Example](img/curios/curios_slots.png)

---

## Getting More Curios Slots

Some specific Curios items grant additional slots of certain types when equipped.

*   **Head:** `Oddeyes Glasses` - When equipped in a Head slot, grants **+2 Head slots**.
    ![Oddeyes Glasses](img/curios/oddeyes_glasses.png)

*   **Back:** `Triple Strip Cape` - When equipped in a Back slot, grants **+3 Back slots**.
    ![Triple Strip Cape](img/curios/triple_strip_cape.png)

*   **Hands:** `Infinity Glove` - When equipped in a Hands slot, grants **+5 Ring slots** and **+1 Charm slot**.
    ![Infinity Glove](img/curios/infinity_glove.png)

*   **Belt:** `Leather Belt` - When equipped in the Belt slot, grants up to **+8 Charm slots**.
    ![Leather Belt](img/curios/leather_belt.png)

---

## Curios by Slot Type

Here are examples of items that fit into specific Curios slots available in ATMA:

### Spell Focus Slot

![Spell Focus Slot Icon](img/arsnouveau/spell_focus_slot.png)

*   **Description:** A dedicated slot primarily used by **Ars Nouveau** for its `Spell Foci`.
*   **Functionality:** Equipping a Focus provides passive benefits and enhances certain spells or schools of magic.
*   **Compatibility:** Items tagged `#curios:an_focus` fit here.
*   **Examples:** `Focus of Earth`, `Focus of Water`, `Focus of Fire`, `Focus of Air`, `Focus of Necromancy`, `Focus of Summoning`, `Focus of Block Shaping`, `Focus of Transmutation` (Ars Technica).
*   **Details:** [Click here for an in-depth explanation of Spell Focus](arsnouveau/README.md/#spell-focus)

### Head Slot

![Head Slot Icon](img/curios/head_slot.png)

*   **Description:** A slot for items worn on the head, often providing utility or visual effects. Items here can typically also be worn in the vanilla helmet armor slot.
*   **Functionality:** Varies greatly depending on the item equipped.
*   **Compatibility:** Items tagged `#curios:head` fit here.
*   **Examples:**

    ![Various Head Slot Items](img/curios/head_slot_items.png)

    #### 1. Occultism
    *   `Otherworld Goggles`: Grants the permanent **Third Eye** effect, allowing the wearer to see hidden Otherworld blocks and entities related to Occultism. This ability, referred to as "seeing beyond the veil," is normally temporary and achieved by consuming `Demon's Dream` herbs.

    #### 2. The Bumblezone
    *   `Flower Headwear`: Prevents bees from becoming angry and attracts them when worn in the *armor* slot. **Functionality may not work correctly when equipped in the Curios slot**, and it provides no visual change in the Curios slot either.

    #### 3. Ars Nouveau & Addons
    *   **(Ars Technica)** `Spy Monocle`: Allows zooming in by pressing ++g++ (configurable).
    *   `Alchemist's Crown`: Allows opening a potion radial menu by pressing ++g++ (configurable) when `Potion Flasks` are in the inventory.
        ![Alchemist's Crown Radial Menu](img/curios/alchemist_crown.png)

    #### 4. L2Hostility
    *   `Oddeyes Glasses`: When equipped in a Head slot, grants **+2 Head slots**.
    *   `Detector Glasses`: Allows you to see invisible mobs and see mobs even when affected by Blindness or Darkness. Additionally, while holding a `Hostility Detector` in the off-hand, you can use it to clear the difficulty in an area. [Click here for more information](l2hostility.md/#ways-to-decrease-player-difficulty).

    #### 5. Create
    *   `Engineer's Goggles`: Augments your HUD with information about placed Create components (Stress, Capacity, item/fluid content).

    #### 6. Hexerei
    *   `Reading Glasses`: Allows zooming in by pressing ++z++ (configurable).

    #### 7. Artifacts
    *Note: Artifacts share experience earned and level up through use.*

    ![Head Artifact Examples](img/curios/head_artifacts.png)

    *   `Whoopee Cushion`: Grants`Flatulence`. Chance to knock back nearby entities and apply nausea when taking damage or crouching frequently.
    *   `Angler's Hat`: Grants `Generous Catch`. Chance to increase the amount of catch received while fishing, potentially repeating multiple times.
    *   `Cowboy Hat`: Grants `Gallop` (Increases mount speed, jump height, safe fall height) and `Lasso` (Activated: Ride/control any mob temporarily, 1m cooldown).
    *   `Night Vision Goggles`: Grants `Gamma Vision`. Enhances brightness and reduces Blindness/Darkness effectiveness.
    *   `Novelty Drinking Hat` / `Plastic Drinking Hat`: Grants `Quick Drink` (Increases drinking speed) and `Life-Giving Sip` (Replenishes hunger when drinking).
    *   `Snorkel`: Grants `Clear Vision` (Removes water fog) and `Breath Control` (Grants Water Breathing upon submersion).
    *   `Superstitious Hat`: Grants `Big Loot`. Chance to add temporary Looting levels on kill, potentially repeating.
    *   `Villager Hat`: Grants `Innocent Appearance` (Prevents Iron Golem aggression) and increases trading discounts.

    #### 8. Reliquified Twilight Forest
    *Note: Relics share experience earned and level up through use.*

    ![Head Reliquified Twilight Forest Examples](img/curios/reliquified_tf_head.png)

    *   **`Lich Crown`**:
        *   Grants `Bone Pact`: All skeletons become friendly.
        *   Allows socketing `Soulbound Gems` (up to 18 total). Unique gems add abilities, duplicates level them up. Insert/remove via ++rbutton++.
        *   **Available Gems:**
            *   `Absorption Gem` (`Will to Live`): When health is below 20%, drains a percentage of max health from nearby targets for 5s (31.2% drain, 14 block range at max level). 2s cooldown.
            *   `Necromancy Gem` (`Risen Servants`): Every 4s (at max level), spawns a mini-zombie (up to 20 total) dealing 12 damage (at max level).
            *   `Shielding Gem` (`Fortification`): Every 0.7s (at max level), creates a shield blocking one directed attack (up to 23 shields active).
            *   `Frost Gem` (`Frostbite`): Attacks apply stacking frostbite for 14s (at max level). After 7s, target takes 1 armor-piercing damage every 2s.
            *   `Twilight Gem` (`Twilight Touch`): Pressing LMB while looking at a target launches a projectile (3 blocks/sec) dealing 13 damage (at max level). Doesn't work in melee range.
    *   **`Thorn Crown`**:
    *   Grants `Goblin Sense` (Activated): Worsens vision but detects valuable ores within 16 blocks (at max level). Can store up to 5 ore blocks internally (++rbutton++ with ore in inventory) to ignore those specific blocks. Extract stored ore with an empty cursor.
        *   Grants `Oak Skin`: Grants full resistance to 'thorn' damage.
    *   **`Deer Antler`**:
        *   Grants `Acupuncture`: Chance to paralyze on touch/unarmed hit.
        *   Grants `On the Horns!` (Activated): Impale small creatures on antlers, preventing them from attacking.

    #### 9. Reliquified Ars Nouveau
    *Note: Relics share experience earned and level up through use.*

    ![Head Reliquified Ars Nouveau Examples](img/curios/reliquified_ars_head.png)

    *   `Horn of the Wild Hunter` (`Wild Hounds`): Summons 2 invulnerable wolves that fight alongside the player, dealing bonus damage.
    *   `Whirlisprig Petals` (`Ascension`): Holding jump lifts player; automatically grants Slow Falling when falling.

    #### 10. Aesthetic ONLY Items
    *(These provide no functional benefit when equipped)*

    ![Head Aesthetic ONLY Item Examples](img/curios/aesthetic_head.png)

    *   Trophies from **Twilight Forest**: `Twilight Lich Trophy`, `Snow Queen Trophy`, `Questing Ram Trophy`, `Naga Trophy`, `Alpha Yeti Trophy`, `Minoshroom Trophy`, `Knight Phantom Trophy`, `Hydra Trophy`, `Ur-Ghast Trophy`
    *   Other **Twilight Forest**: `Moonworm`, `Cicada`, `Firefly`
    *   **Cataclysm**: `Aptrgangr Head`, `Draugur Head`, `Kobolediator Head`
    *   **Starbunclemania**: `Whirly Propeller`, `Alakakrinas Hat`, `Drygme Horns`, `Sea Bunny`, `Starby Ears`

### Necklace Slot

![Necklace Slot Icon](img/curios/necklace_slot.png)

*   **Description:** A slot for necklaces, amulets, and pendants, often providing passive buffs or utility effects.
*   **Functionality:** Varies greatly depending on the item equipped.
*   **Compatibility:** Items tagged `#curios:necklace` fit here.
*   **Examples:**

    ![Necklace Slot Items](img/curios/neck_items.png)

    #### 1. Ars Nouveau
    *   `Amulet of Mana Boost`: Increases maximum mana by +50.
    *   `Amulet of Mana Regen`: Increases mana regeneration rate by +3.

    #### 2. Reliquary
    *   `Coin of Fortune`: Automatically draws in nearby items and experience orbs. Can be activated (++shift+rbutton++) and held (++rbutton++) for a larger vacuum effect.

    #### 3. Nature's Aura
    *   `Amulet of Wrath`: *(No tooltip provided - likely enhances combat capabilities)*.

    #### 4. Iron's Spells 'n Spellbooks & Addons

    ![Iron's Spells 'n  Spellbooks Necklaces](img/curios/irons_necklaces.png)

    *   `Amulet of Concentration`: Makes long-cast spells uninterruptible.
    *   `Conjurer's Talisman`: Increases summon damage by 10%.
    *   `Heavy Chain`: Increases spell resistance by 15%.
    *   `Amethyst Resonant Charm`: Increases mana regeneration by 15%.
    *   `Amulet of Teleportation`: *(No tooltip provided - likely enhances teleportation spells or grants a teleport ability)*.
    *   **(Traveloptics)** `Energy Unbound Necklace`: Allows free look and slow movement while casting Death Laser (reduces laser damage).
    *   **(Traveloptics)** `Sigil of the Spider Sorcerer`: Allows wall climbing while Aspect of the Spider is active; hitting enemies while active poisons them.
    *   **(Traveloptics)** `Amulet of Spectral Shift`: Spectral Blink spell now teleports the *target* entity to your location while crouching.
    *   **Jewelry Crafting:** `Simple Amulets`, `Simple Chains`, `Amulet of Protection` can be crafted. *(Refer to Iron's Spells 'n Spellbooks Guide - WIP)*.

    #### 5. Silent Gear
    *   **Special Mention:** `Necklace Blueprint`. Used to craft necklaces using Silent Gear's material system. *(Refer to Silent Gear Guide - WIP)*.

    #### 6. Artifacts
    *Note: Artifacts share experience earned and level up through use.*

    ![Necklace Artifact Examples](img/curios/necklace_artifacts.png)

    *   **`Flame Pendant`**: Grants `Fiery Defense` (Chance to ignite attackers).
    *   **`Shock Pendant`**: Grants `Electric Resistance` (Immunity to lightning) and `Lightning Defense` (Chance to strike attackers with lightning).
    *   **`Thorn Pendant`**: Grants `Poisonous Defense` (Chance to reflect damage and poison attackers).
    *   **`Panic Necklace`**: Grants `Panic` (Increases movement speed based on nearby hostile mobs targeting you).
    *   **`Cross Necklace`**: Grants `Invincibility` (Increases invulnerability duration after taking damage).
    *   **`Scarf of Invisibility`**: Grants `Silent Step` (Grants invisibility, breaks temporarily on interaction or when targeted).
    *   **`Charm of Shrinking`**: Grants `Compression` (Reduces player size).
    *   **`Charm of Sinking`**: Grants `Anchor` (Increases sinking speed) and `Diver` (Restores air while on underwater floor).
    *   **`Lucky Scarf`**: Grants `Treasure Hunter` (Chance to add temporary Luck levels when mining, potentially repeating).

    #### 7. Reliquified Amulets
    *Note: Relics share experience earned and level up through use.*

    ![Relic Necklace Examples](img/curios/relic_necklaces.png)

    *   **`Reflecting Necklace`**: Accumulates damage taken, then explodes dealing damage and stunning targets based on stored damage.
    *   **`Jellyfish Necklace`**: Grants `Power over the sea` (No sinking), `Electrical Discharge` (Damage on collision), and `Paralysis` (Paralyzes on discharge).
    *   **`Holy Locket`**:
        *   `Faith` (Toggleable): **Holiness (Red):** Steals healing from nearby entities. **Unholiness (Blue):** Deals damage to nearby entities based on healing received.
        *   `Penitence`: Ignites undead and increases damage dealt to them.
        *   `Ascension`: Killing targets grants temporary stacking immortality.

### Back Slot

![Back Slot Icon](img/curios/back_slot.png)


*   **Description:** A slot for items worn on the back, such as capes, backpacks, quivers, or wings. These often provide utility, storage, or movement enhancements. Items here can typically also be worn in the vanilla chestplate armor slot if they are armor pieces (like Elytra).
*   **Functionality:** Varies greatly, including inventory expansion, ranged weapon utility, flight, or passive buffs.
*   **Compatibility:** Items tagged `#curios:back` fit here.
*   **Examples:**

    ![Back Slot Items](img/curios/back_slot_items.png)

    #### 1. L2Backpacks
    *   `Backpack`: Provides extra inventory storage accessible via a hotkey.
    *   `Quiver`: Automatically supplies arrows to bows, stores different arrow types.
    *   `Tool Swap`: Allows quick swapping between tools via a menu.
    *   `Armor Swap`: Allows quick swapping between armor pieces via a menu.
    *   `Suit Swap`: Allows quick swapping between full gear sets via a menu.
    *   *(Note: A dedicated guide for L2Backpacks with detailed functionality is planned).*

    #### 2. L2Hostility
    *   `Triple Strip Cape`: When equipped in a Back slot, grants **+3 Back slots**.

    #### 3. Sophisticated Backpacks
    *   `Backpack`: Provides highly configurable and upgradeable extra inventory storage accessible via hotkey or placing the backpack. Can be equipped in the Back slot.
    *   *(Note: A dedicated guide for Sophisticated Storage/Backpacks with detailed functionality is planned).*

    #### 4. Silent Gear
    *   **Special Mention:** `Elytra Blueprint`. Used to craft Elytra using Silent Gear's material system, allowing for customization of flight properties and durability. *(Refer to Silent Gear Guide - WIP for crafting details)*.

    #### 5. Relics
    *Note: Relics share experience earned and level up through use.*

    ![Relics Back](img/curios/relics_back.png)

    *   **`Midnight Robe` (Combined Relic)**:
        *   Grants `Vanish`: Grants complete invisibility and increases movement speed (up to 157% at max level) when the light level is 12 or less.
        *   Grants `Betrayal`: Attacking while `Vanish` is active deals increased damage (up to 250% at max level), marks a circle (10 blocks radius at max level) around the target, and dispels invisibility. `Vanish` cannot be reactivated until the wearer leaves the circle.
    *   **`Elytra Booster`**:
        *   Grants `Acceleration`: Uses furnace fuel added to the relic to fill an internal buffer (max 350 units at max level). Activating the ability while flying with elytra increases flight speed (up to 48 blocks/sec at max level) by consuming fuel.

    #### 6. Reliquified Ars Nouveau
    *Note: Relics share experience earned and level up through use.*

    ![Reliquified Ars Nouveau Back](img/curios/reliquified_ars_back.png)

    *   **`Whirlisprig Broom`**:
        *   Grants `Witch's Call`: Summons a controllable broom (standard movement keys) with a max flight height (80 blocks above ground at max level). Broom has health (20 at max level, regenerates every 5s), disappears if health depletes (1 min cooldown). Sprinting consumes mana (45/sec at max level) and increases speed (by 300% at max level).
    *   **`Spiked Cloak`**:
        *   Grants `Boiling Point`: When taking damage equal to a percentage of max health (60% at max level), fires several spikes dealing damage (15 each at max level). If triggered again within a time window (30s at max level), spike damage doubles and the cooldown resets. Bonus damage resets if the timer expires.
    *   **`Cloak of Concealment`**:
        *   Grants `Mana Barrier`: Absorbs incoming damage by consuming mana (25 per point of damage at max level). If mana drops too low for absorption, the ability goes on cooldown (10 seconds at max level).

    #### 7. Reliquified Twilight Forest
    *Note: Relics share experience earned and level up through use.*

    ![Reliquified Twilight Forest Back](img/curios/reliquified_tft_back.png)

    *   **`Charm Backpack`**:
        *   Grants `Charm Storage`: Allows storing charms (up to 13 at max level) inside the backpack (++rbutton++ on backpack with charm). Prevents charm destruction upon activation, instead putting the backpack on cooldown (2.5 minutes per charm level at max level). Extract charms with an empty cursor. Only for base Twilight Forest Charms (`Charm of Life` and `Charm of Keeping`)
    *   **`Steel Cape`**:
        *   Grants `Invulnerability`: Reduces incoming damage mitigated by armor by a flat amount (2 points at max level). If damage isn't fully blocked, has a chance (50% at max level) to launch a steel orb at the attacker, dealing damage (12 at max level) and stunning (5 seconds at max level).
    *   **`Scaled Cloak`**:
        *   Grants `Grip`: Allows climbing walls for a duration (25 seconds at max level), then slowly slide down.
        *   Grants `Elusive Stare`: When taking damage, has a chance (125% at max level - likely guarantees activation) to make the attacker miss if the player maintains eye contact.
    *   **`Invisibility Cloak`**:
        *   Grants `Imperial Attire`: Hides the appearance of equipped armor (cosmetic).
        *   Grants `Camouflage`: Grants full invisibility after standing still or sneaking without interruption for a duration (1 second at max level).
    *   **`Chromatic Cloak`**:
        *   Grants `Spectrum Magic`: Stores colored wool (up to 16 slots, 48 units each at max level). Each active wool color grants a specific effect for a duration (29 seconds at max level), consuming one unit. Insert/extract wool via ++rbutton++.
        *   Grants `Color Focus`: Increases the effect level based on the number of identical-colored wool slots (up to level 14 at max level).
        *   **Wool Effects:**
            *   White: Levitation Resistance
            *   Light Gray: Reflection (Reflect projectiles?)
            *   Gray: Weather Resistance
            *   Black: Spider Climb
            *   Brown: Haste
            *   Red: Strength
            *   Orange: Fire Resistance
            *   Yellow: Reach
            *   Lime: Luck
            *   Green: Poison Resistance
            *   Cyan: Water Breathing
            *   Light Blue: Speed
            *   Blue: Night Vision
            *   Purple: Saturation
            *   Magenta: Regeneration
            *   Pink: Health Boost



---

## How to Equip Curios Items

1.  Press the **Curios key** (Default key: 'G') to open the Curios slots GUI.
2.  Identify the appropriate slot type for the item you want to equip (e.g., Head, Back, Necklace, Hands, Belt, Charm, Ring, Focus).
3.  Drag the desired Curios item from your main inventory into a compatible empty slot in the Curios GUI.
4.  The item is now equipped, and its effects (if any) should be active!

---

> **Curios API** | [CurseForge Link](https://www.curseforge.com/minecraft/mc-mods/curios)
