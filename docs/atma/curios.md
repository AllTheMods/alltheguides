---
title: Curios and Relics
description: A Guide for Curios Slots and Relics in All the Magic - Arcana (ATMA)
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

![Spell Focus Slot Icon](img/curios/spell_focus_slot.png)

*   **Description:** A dedicated slot primarily used by **Ars Nouveau** for its `Spell Foci`.
*   **Functionality:** Equipping a Focus provides passive benefits and enhances certain spells or schools of magic.
*   **Compatibility:** Items tagged `#curios:an_focus` fit here.
*   **Examples:**

    ![Spell Focus Items](img/curios/spell_focus_items.png)

    #### Common Mechanics for Elemental Focus (Earth, Water, Fire, Air)
    *   **Attunement:** Each elemental focus is attuned to a specific school of magic (e.g., Focus of Earth -> Earth School).
    *   **Amplification & Discount:** While equipped, spells (glyphs) belonging to the attuned school are generally stronger and/or cost less mana.
    *   **Lesser Focus Drawback:** The basic ("Lesser") version of these elemental Focus often weakens spells from the *other* three elemental schools (Fire, Water, Earth, Air).
    *   **Major Focus Bonus:** An upgraded version typically provides an additional, more powerful bonus under specific conditions, likely alongside the amplification/discount.

    #### 1. Ars Nouveau - Elemental Foci
    *   **`Focus of Earth`**:
        *   **Attunement:** Earth
        *   **Lesser Drawback:** Weakens Fire, Water, Air glyphs.
        *   **Major Bonus:** Grants Mana Regen I while the wearer is below Y=0 (deep underground).
        *   **Empowered Effects:**
            *   `Poison Spores` / `Grow`: Deals damage to Undead mobs, chance to spawn a `Spore Blossom`.
            *   `Gravity` (Augmented with `Sensitive`): Creates a gravity well pulling entities towards the center (filter-compatible).
            *   Passively grants Knockback Resistance.
            *   Boosts natural and instant Healing effects received by 1.5x.
    *   **`Focus of Water`**:
        *   **Attunement:** Water
        *   **Lesser Drawback:** Weakens Fire, Earth, Air glyphs.
        *   **Major Bonus:** Grants Mana Regen I while wet; OR Mana Regen II + Dolphin's Grace effect while swimming.
        *   **Empowered Effects:**
            *   `Freeze`: Applies stacking "Freezing" buildup, eventually inflicting "Frozen" status (short duration, stops healing).
            *   `Freeze` (Used after `Conjure Water`): Turns the conjured water into Ice blocks.
            *   `Summon Steed`: Summons a rideable Dolphin instead (build speed by timing jumps out of water).
            *   Converts Drowning damage dealt *to* water creatures into Magic damage.
    *   **`Focus of Fire`**:
        *   **Attunement:** Fire
        *   **Lesser Drawback:** Weakens Water, Earth, Air glyphs.
        *   **Major Bonus:** Grants Spell Damage II while the wearer is on fire or in lava.
        *   **Empowered Effects:**
            *   `Ignite`: Inflicts "Magic Burn".
            *   Allows `Flare` spell to damage/spread even on fire-resistant mobs.
            *   Allows magic damage to partially pierce armor.
            *   Makes Earth damage less effective against the target (negative synergy).
            *   `Summon Steed`: Summons a rideable Strider instead.
            *   `Ignite` + `Evaporate` Combo: Sublimates (destroys) Ice blocks.
    *   **`Focus of Air`**:
        *   **Attunement:** Air
        *   **Lesser Drawback:** Weakens Fire, Water, Earth glyphs.
        *   **Major Bonus:** Grants Mana Regen I while the wearer is above Y=200 OR while under the "Shocked" effect.
        *   **Empowered Effects:**
            *   `Launch` (Augmented with `Extend Time`): Applies the `Levitate` effect instead of just launching.
            *   `Cut`: Gives a chance to drop a mob's head or skull if `Cut` deals the killing blow.

    #### 2. Ars Nouveau - Other Foci
    *   **`Focus of Necromancy`**:
        *   **Mechanics:** Does not follow standard elemental attunement/drawback rules.
        *   **Effects:**
            *   Summoned Wolves, Undead, and Vexes will revive once upon death if the summoner is wearing the focus, returning with "blood lust".
            *   Summoned undead specifically will cast Homing spells when you do.
            *   Summoned undead specifically will heal you each time they kill an enemy.
    *   **`Focus of Summoning`**:
        *   **Mechanics:** Does not follow standard elemental attunement/drawback rules. Special focus for enhancing summons.
        *   **Effects:**
            *   Grants summons (from spells) additional duration, strength, and speed.
            *   Deals damage to enemies that kill your summons (similar to Thorns for summons).
            *   Casting spells that target you (like `Self` or `Orbit` casting methods) will also cast a copy on your nearby summons.
    *   **`Focus of Block Shaping`**:
        *   **Mechanics:** Does not follow standard elemental attunement/drawback rules. Special focus for block manipulation spells.
        *   **Effects:**
            *   **Impact Damage:** Blocks moved by spells (`Launch`, `Gravity`, `Pull`, `Knockback`, etc.) now deal damage to entities they collide with. Damage scales with your Spell Damage stat, the block's hardness, and the block's speed.
            *   **Spell Continuation:** Modifying, creating, or moving a block causes the remainder of the spell sequence to target the new or moving block, rather than the original target point.
                *   *Example (Creation):* `Freeze` -> `Break` will now correctly target the newly formed ice block with `Break`.
                *   *Example (Movement):* `Conjure Mageblock` -> `Launch` -> `Ignite` will launch the block, and the `Ignite` effect will apply to the moving block.
            *   Affects glyphs like `Conjure Mageblock`, `Freeze`, `Break`, `Exchange`, `Place Block`, `Launch`, `Pull`, etc.
            *   Synergizes heavily with `Area of Effect` (AoE) augmentation to manipulate or weaponize many blocks simultaneously.

    #### 3. Ars Technica
    *   **`Focus of Transmutation`**:
        *   **Mechanics:** Does not follow standard elemental attunement/drawback rules. Focus for item processing and enhancement glyphs.
        *   **Core Function:** Augments spells with the `Luck` effect and improves specific processing glyphs.
        *   **Provides the following bonuses:**
            *   2x Speed: For `Press`, `Polish`, and `Whirl` glyphs.
            *   2x Items Processed: For `Press` and `Polish` glyphs (processes two items per operation).
            *   2x Chance-Based Outputs: For `Obliterate` and `Whirl` glyphs (e.g., doubling ore dust chance).
            *   2x Damage: For the `Obliterate` glyph.
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

### Body Slot

![Body Slot Icon](img/curios/body_slot_icon.png)

*   **Description:** Currently only one item available.
*   **Functionality:** Currently only one item available.
*   **Compatibility:** Items tagged `#curios:body` fit here.
*   **Examples:**

    ![Body Slot Items](img/curios/body_slot_items.png)

    #### 1. Reliquary
    *   `Twilight Cloak`: Makes you invisible in darkness.


### Bracelet Slot

![Bracelet Slot Icon](img/curios/bracelet_slot.png)

*   **Description:** A slot typically used for bracelets or bangles worn on the wrist. These often provide passive buffs related to specific magic schools or attributes. By default, players have **two** bracelet slots available.
*   **Functionality:** Primarily provides passive statistical bonuses, often enhancing specific types of magic, movement speed in certain conditions, or granting resistances.
*   **Compatibility:** Items tagged `#curios:bracelet` fit here.
*   **Examples:**

    ![Various Bracelet Slot Items](img/curios/bracelet_slot_items.png)

    #### 1. Ars Nouveau

    ![Ars Nouveau Bracelet](img/curios/ars_bracelet.png)

    *   **`Enchanter's Bangle`**: Base item used to craft elemental/themed bangles. Provides a slight boost to overall spellcasting.
    *   **`Bangle of Fire`**:
        *   Boosts the damage of Fire spells more significantly than the base bangle.
        *   Arms are engulfed in fire, setting enemies on fire when hit.
        *   Grants a passive speed boost while in hot biomes.
    *   **`Bangle of Water`**:
        *   Boosts the damage of Water spells more significantly than the base bangle.
        *   Arms chill the air, freezing enemies on hit.
        *   Grants a passive speed boost (+50% swim speed) in water and rain.
    *   **`Bangle of Air`**:
        *   Boosts the damage of Air spells more significantly than the base bangle.
        *   Arms spark with the element, giving a passive boost to speed (+60%) and attack knockback (+1.2).
    *   **`Bangle of Earth`**:
        *   Boosts the damage of Earth spells more significantly than the base bangle.
        *   Plants blossom on arms, inflicting snare on enemies hit.
        *   Grants immunity to cactus and berry bush damage.
        *   Grants knockback resistance (+30%).
    *   **`Bangle of Summoning`**:
        *   Boosts the damage of Summoning spells (+2 Summoning Power).
        *   Summons follow arm movements, targeting whatever the player hits with increased damage.
    *   **`Bangle of Anima`**:
        *   Boosts the damage of Anima spells.
        *   Represents a cycle of life and death: randomly heals or withers enemies hit.
        *   Grants a small health boost (+4 Max Health).

    #### 2. Iron's Spells 'n Spellbooks (Addon: Traveloptics)
    *   **`Nightstalker's Band`**:
        *   Allows the `Reversal` spell to be cast without a weapon.
        *   Reflecting a projectile grants the `Assassin` effect for 5 seconds (boosts movement speed and greatly enhances attack damage). Effect ends upon striking an entity.
    *   **`Azure Ignition Bracelet`**:
        *   Permanently ignites Ignis-themed spells with soul fire, increasing their damage.

    #### 3. Silent Gear
    *   **Special Mention:** `Bracelet Blueprint`. Used to craft bracelets using Silent Gear's material system, allowing for customization of effects and stats. *(Refer to Silent Gear Guide - WIP for crafting details)*.

    #### 4. Artifacts
    *Note: Artifacts share experience earned and level up through use.*
    *   **`Withered Bracelet`**:
        *   Grants `Wither Resistance`: Complete immunity to wither damage.
        *   Grants `Withering Touch`: Chance (up to 80% at max level) to apply Wither effect to attacked targets for a duration (12 seconds at max level).
    *   **`Onion Ring`**:
        *   Grants `Miner's Hunger`: Increases block mining speed (by 4.5% at max level) per unit of the player's saturation.
        *   Grants `Raw Appetite`: When mining blocks, has a chance (30% at max level) to restore 1 hunger point and 0.5 saturation.

    #### 5. Reliquified Ars Nouveau
    *Note: Relics share experience earned and level up through use.*
    *   **`Flaming Bracer` (Combined Relic)**:
        *   *(Base)* Grants `Pyrophagy`: Complete immunity to magical fire damage.
        *   *(Gem)* Grants `Pyrokinesis`: When dealing melee damage to a burning target, has a chance (90% at max level) to release magical fire. If successful, the ability repeats, releasing additional bursts (up to 9 total triggers at max level).


### Hostility Curse Slot

![Hostility Curse Slot Icon](img/curios/hostility_curse_slot.png)

*   **Description:** A specific slot added by **L2Hostility**, primarily intended for its "Curse" items. These items interact directly with the L2Hostility mod's difficulty and loot mechanics, often increasing difficulty in exchange for potential rewards or altering how loot/traits drop. Many items fitting here can *also* be equipped in the standard `Charm` slot, but some effects might differ or only apply when in the Curse slot.
*   **Functionality:** Modifies L2Hostility mechanics, usually involving increased difficulty, altered loot tables, trait acquisition, or immunity to certain negative effects.
*   **Compatibility:** Items tagged `curios:hostility_curse` fit here. Note that `Abyssal Thorn`, `Abrahadabra`, and `Greed of Nidhoggur` *only* fit in this slot, while others may also fit in `curios:charm`.
*   **Examples:**

    ![Various Hostility Curse Items](img/curios/hostility_curse_items.png)

    #### 1. L2Hostility
    *   **Looting Charms (`Unpolished`, `Magical`, `Chaotic`, `Miraculous`)**:
        *   Enables some hostility trait drops (check JEI for specifics for each tier).
        *   Can be worn in **Charm** or **Curse** slots.
    *   **`Curse of Envy`**:
        *   Get trait items when killing mobs with traits (2% chance per trait rank).
        *   Increases player difficulty by +50 when worn (either slot).
        *   Can be worn in **Charm** or **Curse** slots.
    *   **`Curse of Greed`**:
        *   Doubles (x2.0) hostility loot drop chance.
        *   Increases player difficulty by +50 when worn (either slot).
        *   Can be worn in **Charm** or **Curse** slots.
    *   **`Curse of Lust`**:
        *   Mobs you kill will drop all their equipped items.
        *   Increases player difficulty by +50 when worn (either slot).
        *   Can be worn in **Charm** or **Curse** slots.
    *   **`Curse of Wrath`**:
        *   Gain 1% attack damage per difficulty level difference against mobs with higher levels.
        *   Grants immunity to Blindness, Darkness, Mining Fatigue, Nausea, Slowness, Weakness.
        *   Increases player difficulty by +50 when worn (either slot).
        *   Can be worn in **Charm** or **Curse** slots.
    *   **`Curse of Sloth`**:
        *   Prevents gaining difficulty by killing mobs.
        *   Prevents mobs you kill from dropping hostility loot.
        *   Can be worn in **Charm** or **Curse** slots.
    *   **`Curse of Gluttony`**:
        *   Get `Bottle of Curse` when killing mobs with a level (2% chance per level).
        *   Can be worn in **Charm** or **Curse** slots.
    *   **`Abyssal Thorn`**:
        *   Mobs get all possible traits at their level.
        *   If `Curse of Envy` is also equipped, mobs will always drop trait symbols for those traits when killed.
        *   Can **only** be worn in the **Curse** slot.

    *   **Currently Unobtainable Items:** *(Note: The following items require traits/materials that are currently disabled or unavailable for crafting in ATMA. This might change in future updates.)*
        *   **`Abrahadabra`**:
            *   When a mob trait tries to apply an effect to you, apply it to surrounding enemies targeting you instead.
            *   Increases player difficulty by +100 when worn.
            *   Can **only** be worn in the **Curse** slot.
        *   **`Curse of Pride`**:
            *   Gain 1% health and 1% attack damage per difficulty level.
            *   Mob traits will be +100% more frequent.
            *   Can be worn in **Charm** or **Curse** slots.
        *   **`Greed of Nidhoggur`**:
            *   Doubles (x2.0) hostility loot drop chance.
            *   Mobs you kill drop +1% loot per mob level.
            *   Increases player difficulty by +100 when worn.
            *   Can **only** be worn in the **Curse** slot.
        *   **`Divinity Cross`**:
            *   Prevents the Cleanse effect from clearing Level 1 beneficial effects.
            *   Can be worn in **Charm** or **Curse** slots.
        *   **`Divinity Light`**:
            *   Keeps your adaptive level at 0.
            *   Can be worn in **Charm** or **Curse** slots.

### Hands Slot

![Hands Slot Icon](img/curios/hands_slot.png)

*   **Description:** A slot for items worn on the hands, typically gloves or other hand-related accessories. These often grant combat bonuses, utility functions, or interact with specific mod mechanics. By default, players have **two** hands slots available.
*   **Functionality:** Varies widely, from accessing remote storage and applying on-hit effects to granting additional Curios slots or modifying damage types/mechanics.
*   **Compatibility:** Items tagged `#curios:hands` fit here.
*   **Examples:**

    ![Various Hands Slot Items](img/curios/hands_slot_items.png)

    #### 1. Occultism
    *   `Storage Accessor` (Storage Remote): Allows remote access to an Occultism storage network (Dimensional Storage Actuator). Requires binding to an actuator first.

    #### 2. Cataclysm Items
    *   `Blazing Grips`: On hit, chance to apply `Blazing Brand` to the target.
    *   `Sticky Gloves`: Blocks the looting mechanic of Koboletons (from Cataclysm).

    #### 3. L2Hostility
    *   `Infinity Glove`: When worn, grants **+5 Ring slots** and **+1 Charm slot**.
    *   `Imagine Breaker`: All melee damage bypasses magical protection. Mobs killed while wearing this will not drop hostility loot.
    *   `Flaming Thorn`: When damaging a mob, inflict Soul Flame for 5 seconds with a level equal to the total number of effects that mob has.
    *   **Currently Unobtainable Items:** *(Note: The following item requires traits/materials that are currently disabled or unavailable for crafting in ATMA. This might change in future updates.)*
        *   `Platinum Star`: All melee damage bypasses damage cooldown. (Can also be worn in **Charm** slot).

    #### 4. Glimmering Tales
    *   `Glove of Thunder`: [Thunder] spell damage bypasses damage cooldown. Reduces Mana Regen by 25% (x0.75 multiplier).
    *   `Glove of Ocean`: [Ocean] spell damage bypasses damage cooldown. Reduces Mana Regen by 25% (x0.75 multiplier).
    *   `Glove of Abyss`: Infuses all spell damage with Abyss damage. Reduces Mana Regen by 50% (x0.5 multiplier).
    *   `Glove of Sorcerer`: Converts all spell damage to magic damage. Increases Magic Damage by +25%.

    #### 5. Relics
    *Note: Relics share experience earned and level up through use.*

    *   **`Rage Glove`**:
        *   Grants `Berserker Rage`: Attacks within 8s of the last add a charge. Increases damage (+15%/charge) but also damage taken (+3.8%/charge). Failing to attack resets charges.
        *   Grants `Phlebotomy`: Increases attack speed (+1.5%) and movement speed (+5%). Grants passive health regen (+0.01% per missing % health).
        *   Grants `Spurt` (Activated): Dashes (up to 32 blocks), igniting, bleeding, and attacking targets in path. Deals bonus damage (+0.5 per Berserker Rage charge), empties charge buffer, then goes on cooldown (6.9s).
    *   **`Ender Hand`**:
        *   Grants `Neutrality`: Makes Endermen neutral towards the wearer.
        *   Grants `End Transposition` (Activated): Swaps the wearer and the target along the line of sight (up to 80 blocks).
    *   **`Wool Mitten`**:
        *   Grants `Mold`: Collect snow (++rmb++ empty hand) to form hardened snowballs (up to 96 units). Hitting a target deals damage (0.5), stuns (0.125s), and freezes (0.125s per unit size). Holding snowballs without the relic equipped freezes the player.

    #### 6. Reliquified Ars Nouveau
    *Note: Relics share experience earned and level up through use.*

    *   **`Archmage Glove`**:
        *   Grants `Dexterous Fingers`: When casting a spell, chance (75% at max level) to cast it again. Repeats do not consume mana but continue until the chance fails (max 5 total repetitions). Works only on pink-colored spells (RGB: 255 25 180).

    #### 7. Reliquified Twilight Forest
    *Note: Relics share experience earned and level up through use.*

    *   **`Giant's Glove`**:
        *   Grants `Giant's Grip`: Increases the size and stats of the held item by 50% (at max level).

    #### 8. Artifacts
    *Note: Artifacts share experience earned and level up through use.*

    *   **`Digging Claws`**:
        *   Grants `Pickaxe Hands`: Reduces the required tool level for all blocks by 1.
        *   Grants `Fast Mining`: Increases block mining speed (by 175% at max level).
    *   **`Feral Claws`**:
        *   Grants `Beast's Fury`: Increases attack speed (by 33% at max level) for each consecutive attack within 3 seconds. Loses 1 charge per second otherwise. Attacking with an unfilled attack speed bar resets accumulated charges.
    *   **`Power Glove`**:
        *   Grants `Power Strike`: Increases damage dealt (by 500% at max level) but enters a 5-second cooldown after each attack.
    *   **`Fire Gauntlet`**:
        *   Grants `Fire Wave`: When attacking, releases several sparks that home in on nearby targets, igniting them (for 10 seconds at max level) and dealing damage (50% of attack damage at max level). The number of sparks is determined by repeated checks of a chance (75% at max level); each successful check releases one additional spark, stopping once a check fails.
    *   **`Pocket Piston`**:
        *   Grants `Concentrated Strike`: Increases knockback in melee attacks (by 100% at max level).
        *   Grants `Long Reach`: Increases maximum interaction range with the world (by 100% at max level).
    *   **`Vampiric Glove`**:
        *   Grants `Life Steal`: Heals the player for a percentage (40% at max level) of the damage dealt.
    *   **`Golden Hook`**:
        *   Grants `Thirst for Knowledge`: Increases experience gained from killing mobs (by 100% at max level).
    *   **`Pickaxe Heater`**:
        *   Grants `Heat Concentration`: Smelts any mined block if possible, consuming one charge from a buffer (capacity 75 units at max level). The buffer regenerates 1 charge every 1 second (at max level).

### Ring Slot

![Ring Slot Icon](img/curios/ring_slot.png)

*   **Description:** A slot for rings worn on the fingers. These commonly provide passive statistical bonuses, often enhancing magical capabilities, regeneration, or specific elemental affinities. Players start with two default ring slots, but this number can be increased by items like the `Infinity Glove`.
*   **Functionality:** Typically grants percentage increases to stats like Maximum Mana, Mana Regeneration, or affinity with specific magical elements (which usually reduces mana costs and potentially increases damage/effectiveness of related spells). Also includes utility rings with unique effects.
*   **Compatibility:** Items tagged `#curios:ring` fit here.
*   **Examples:**

    ![Various Ring Slot Items](img/curios/ring_slot_items.png)

    #### 1. Glimmering Tales
    *   **`Golden Ring`**: +10% Max Mana.
    *   **`Ring of Regeneration`**: +10% Max Mana, +30% Mana Regen.
    *   **`Ring of Nature`**: +10% Max Mana, +10% Earth Affinity, +10% Life Affinity, +10% Flame Affinity, +10% Snow Affinity.
    *   **`Ring of Earth`**: +20% Max Mana, +50% Earth Affinity.
    *   **`Ring of Life`**: +20% Max Mana, +50% Life Affinity.
    *   **`Ring of Thunder`**: +30% Max Mana, +50% Thunder Affinity.
    *   **`Ring of Ocean`**: +20% Max Mana, +50% Ocean Affinity.
    *   **`Ring of Snow`**: +20% Max Mana, +50% Snow Affinity.
    *   **`Ring of Flame`**: +20% Max Mana, +50% Flame Affinity.

    #### 2. L2Hostility
    *   **`Ring of Corrosion`**: When you deal damage, damages the target's equipment by 20% of max durability. When you take damage, damages your equipment by 20% of max durability.
    *   **`Ring of Reflection`**: When a mob trait tries to apply a negative effect on you, apply it to surrounding enemies targeting you instead.
    *   **`Ring of Divinity`**: Grants immunity to magic damage and provides a permanent Cleanse effect.
    *   **`Ring of Ocean`**: You will always be wet.
    *   **`Ring of Healing`**: Heals 3% of max health every second.
    *   **Currently Unobtainable Items:** *(Note: The following items require traits/materials that are currently disabled or unavailable for crafting in ATMA. This might change in future updates.)*
        *   **`Ring of Life`**: Prevents losing more than 90% of your max health in a single instance of damage.
        *   **`Ring of Incarceration`**: When sneaking, applies the Incarceration effect to you and all mobs within your attack range.

    #### 3. Silent Gear
    *   **Special Mention:** `Ring Blueprint`. Used to craft rings using Silent Gear's material system, allowing for customization of effects and stats. *(Refer to Silent Gear Guide - WIP for crafting details)*.

    #### 4. Nature's Aura
    *   **`Ring of Last Chance`** (Death Ring): *(Exact effect TBC - likely prevents death under certain conditions, possibly consuming Aura or durability)*.

    #### 5. Ars Nouveau
    *   **`Ring of Jumping`**: Allows the user to continue jumping in the air, consuming mana with each jump.
    *   **`Ring of Lesser Discount`**: Reduces the mana cost of all spells by 10. Grants +10 Max Mana and +1 Mana Regen.
    *   **`Ring of Greater Discount`**: Reduces the mana cost of all spells by 20. Grants +10 Max Mana and +1 Mana Regen. (Slightly larger discount than the Lesser version).

    #### 6. Occultism
    *   **`Familiar Ring`**: Used to capture and store Occultism Familiars. When equipped with a familiar inside, grants the familiar's passive bonuses. An empty ring provides no benefit. *(Refer to Occultism Guide - WIP for Familiar details)*.

    #### 7. Reliquified Ars Nouveau
    *Note: Relics share experience earned and level up through use.*
    *   **`Mana Ring`**: Grants `Mana Compression`: Increases maximum Mana (+200 points at max level) and Mana Regeneration (+5 points/sec at max level).
    *   **`Ring of Thrift`**: Grants `Reserve`: When casting a spell, chance (50% at max level) that no mana will be consumed.

    #### 8. Cataclysm Spellbooks
    *   **`Leviathan's Blessing`**: +20% Abyssal Spell Power, provides immunity to abyssal effects.

    #### 9. Iron's Spells 'n Spellbooks & Addons
    *   **(Base Mod)** `Signet of the Betrayer`: +10% Eldritch Spell Power. Passive (5s cooldown): Deal extra damage based on target's maximum mana.
    *   **(Base Mod)** `Emerald Stoneplate Ring`: Slain creatures drop +25% experience.
    *   **(Base Mod)** `Ring of Mana`: +100 Max Mana.
    *   **(Base Mod)** `Fireward Ring`: Grants fire immunity.
    *   **(Base Mod)** `Ring of Visibility`: Allows invisible creatures to be seen. (Note: Item ID might still be `invisibility_ring`).
    *   **(Base Mod)** `Poisonward Ring`: Grants poison immunity.
    *   **(Base Mod)** `Ring of Expulsion`: Passive (10s cooldown): When attacked, emit an expulsive burst of air (knockback).
    *   **(Base Mod)** `Ring of Expediency`: +15% Cast Time Reduction.
    *   **(Base Mod)** `Silver Ring`: +25 Max Mana.
    *   **(Base Mod)** `Ring of Recovery`: +15% Cooldown Reduction.
    *   **(Base Mod)** `Frostward Ring`: Grants freezing immunity.
    *   **(Base Mod) Affinity Rings** (`Ring of Fire Affinity`, `Ring of Ice Affinity`, etc.): Crafted by combining a `Ring of No Affinity` with an elemental runestone in the Arcane Anvil. Grants +1 level to spells of the corresponding element (e.g., `Ring of Fire Affinity` boosts Fire spells).
    *   **Jewelry Crafting:** Rings can be crafted using the Jewelry Forge. *(Refer to Iron's Spells 'n Spellbooks Guide - WIP)*.
    *   **(Traveloptics Addon)** `Firestorm Ring`: Transforms meteors from Meteor Storm spell into exploding flare bombs with flame jets. Spell can no longer directly target entities. (Can also fit in **Talent** slot).
    *   **(Traveloptics Addon)** `Aetherial Despair Ring`: Axe Blades of Despair spell gain vertical trajectory and move 50% faster. (Can also fit in **Talent** slot).

    #### 10. Relics
    *Note: Relics share experience earned and level up through use.*
    *   ~~**`Leafy Ring [WIP]`**: Grants `Hide`: *(Functionality currently undefined/Work In Progress)*.~~
    *   **`Chorus Inhibitor`**: Grants `Teleportation Control`: Using a chorus fruit teleports the wearer to a block along the line of sight (up to 96 blocks at max level), then goes on cooldown (5 seconds at max level).
    *   **`Bastion Ring` (Combined Relic)**:
        *   Grants `Recognition`: Makes Piglins neutral. The nearest Piglin indicates the location of a nearby Bastion Remnant.
        *   Grants `Respect`: Each trade with Piglins has multiple 50% chances to yield an additional trade result (up to 11 extra results possible at max level).


### Belt Slot

![Belt Slot Icon](img/curios/belt_slot.png)

*   **Description:** A slot for items worn around the waist, typically belts or sashes. These often provide utility functions, passive buffs, or grant additional Curios slots.
*   **Functionality:** Can range from granting extra Charm slots, providing movement abilities like levitation, giving random potion effects, or offering remote access to storage systems.
*   **Compatibility:** Items tagged `#curios:belt` fit here.
*   **Examples:**

    ![Various Belt Slot Items](img/curios/belt_slot_items.png)

    #### 1. Ars Nouveau & Addons
    *   **(Base Mod)** `Belt of Levitation`: Allows the user to levitate a moderate distance. Sneak while falling or jumping to rise. Reduces a small amount of fall damage while worn.
    *   **(Base Mod)** `Belt of Unstable Gifts`: Occasionally grants a random positive potion effect for a short duration, with varying strengths.
    *   **(Ars Additions)** `Warp Index`: Bind to an Ars Nouveau Storage Lectern (++lshift+rbutton++) to remotely access its stored Spell Tomes via a keybind. Works only within the **same dimension** as the Lectern, which must be chunk-loaded.
    *   **(Ars Additions)** `Stabilized Warp Index`: Functions like the Warp Index but works **across dimensions**. Requires the Storage Lectern to be chunk-loaded.

    #### 2. Occultism
    *   `Surprisingly Substantial Satchel`: Acts as portable storage, linked to the player's Occultism Dimensional Storage system. Requires binding.

    #### 3. Nature's Aura
    *   `Aura Cache`: Stores a small amount of Aura that the player can use.
    *   `Aura Trove`: Stores a larger amount of Aura than the Aura Cache.

    #### 4. Reliquary
    *   `Charm Belt`: Holds mob charms (e.g., Creeper Charm, Skeleton Charm). Exact function TBC (likely prevents mob spawns or grants effects).

    #### 5. Artifacts
    *Note: Artifacts share experience earned and level up through use.*
    *   **`Helium Flamingo`**: Grants `Air Swimmer`: When performing a double jump, allows floating in the air (up to 15 seconds at max level). Movement speed in air is proportional to swimming speed plus a bonus (90% at max level).

    #### 6. Relics
    *Note: Relics share experience earned and level up through use.*
    *   **`Drowned Belt` (Combined Relic)**:
        *   *(Base)* Grants `Load Capacity`: Increases the maximum number of amulet equipment slots (+12 at max level).
        *   *(Gem)* Grants `Dead Height`: Reduces swimming speed (by 0% at max level - no reduction) and increases sinking speed (by 0% at max level - no increase). *(Note: Values might be bugged or intended to be non-negative)*.
        *   *(Gem)* Grants `Water Flows`: Increases damage dealt by the player underwater (by 400% at max level).
        *   *(Gem)* Grants `Water Attraction`: Allows the trident's Riptide enchantment to be used without rain or water, adding a cooldown (0 seconds per enchantment level at max level).
    *   **`Hunter Belt` (Combined Relic)**:
        *   *(Base)* Grants `Load Capacity`: Increases the maximum number of amulet equipment slots (+12 at max level).
        *   *(Gem)* Grants `Training`: Increases the damage dealt by the wearer's pets (by 500% at max level).
    *   **`Leather Belt`**:
        *   Grants `Load Capacity`: Increases the maximum number of amulet equipment slots (+13 at max level).


### Feet Slot

![Feet Slot Icon](img/curios/feet_slot.png)

*   **Description:** A slot for items worn on the feet, such as boots, shoes, or flippers. These typically provide movement-related benefits, environmental interactions, or defensive perks. Can often be worn in the vanilla boots armor slot as well.
*   **Functionality:** Enhances movement speed (running, swimming, on specific blocks), allows walking on liquids or hazardous blocks, grants jump boosts, reduces fall damage, or provides resistances/utility effects.
*   **Compatibility:** Items tagged `#curios:feet` fit here.
*   **Examples:**

    ![Various Feet Slot Items](img/curios/feet_slot_items.png)

    #### 1. Artifacts
    *Note: Artifacts share experience earned and level up through use.*
    *   **`Strider Shoes`**: Allows standing on lava while sneaking. Grants protection against hot floor damage (e.g., magma blocks).
    *   **`Aqua-Dashers`**: Allows walking on fluids (water, lava) while sprinting.
    *   **`Rooted Boots`**: Grants `Herbivory`: Every 1.7 seconds (at max level), transforms the grass block beneath the player into dirt, restoring 1 hunger and saturation point.
    *   **`Flippers`**: Grants `Fish Tail`: Increases the player's swimming speed (by 140% at max level).
    *   **`Steadfast Spikes`**:
        *   Grants `Clinging Claws`: Allows slow wall sliding, negating fall damage.
        *   Grants `Grip`: Increases resistance to knockback and slippery blocks (by 75% at max level).
    *   **`Snowshoes`**:
        *   Grants `Light Step`: Allows walking on powder snow without sinking.
        *   Grants `Snow Walker`: Increases movement speed on snow (by 80% at max level).
    *   **`Running Shoes`**: Grants `High Stride`: Increases the player's running speed (by 240% at max level).
    *   **`Kitty Slippers`**:
        *   Grants `Cat's Gaze`: Scares away Creepers and Phantoms near the player.
        *   Grants `Soft Paws`: Increases safe falling height (by 20 blocks at max level).
        *   Grants `Nine Lives`: Has a chance (35% at max level) to save the player from fatal damage, leaving them with 1 health point.
    *   **`Bunny Hoppers`**: Grants `Jumper`: Allows high jumps by continuously holding the jump key (up to 0.75 seconds charge at max level).

    #### 2. Relics
    *Note: Relics share experience earned and level up through use.*
    *   **`Aqua Walker`**: Grants `Moisture Resistance`: Allows walking on water for a period. After time runs out, boots sink, pulling the wearer down. Requires drying away from water (drying time depends on saturation level).
    *   **`Magma Walker` (Combined Relic)**:
        *   Grants `Heat Resistance`: Suppresses damage from hot blocks.
        *   Grants `Fiery Tread`: Allows walking on lava for a time (100 seconds at max level) without sinking or taking damage. After time runs out, boots overheat, dealing damage proportional to overheating level. Requires cooling away from lava (cooling time depends on overheating level).
    *   **`Ice Skates` (Combined Relic)**:
        *   Grants `Skating`: Increases movement speed on ice (by 87% per second of sliding at max level). Modifier stops increasing if sliding duration exceeds 10 seconds.
        *   Grants `Ram`: Upon collision with targets while `Skating`, deals damage (5 per second of sliding at max level).
    *   **`Ice Breaker` (Combined Relic)**:
        *   Grants `Sustainability`: Increases fall speed, boosts knockback resistance (by 100% at max level), and removes sliding on blocks.
        *   Grants `Earthquake`: Prolonged use while falling until landing creates a shockwave (radius 20 blocks at max level), dealing damage (up to 17.5 at max level) and knocking back targets. Power depends on fall distance.
    *   **`Roller Skates`**: Grants `Acceleration`: Increases movement speed (by 130% per second of movement at max level). Modifier stops increasing if movement duration exceeds 21 seconds. All blocks become slippery.
    *   **`Amphibian Boot` (Combined Relic)**:
        *   Grants `Fins`: Increases swimming speed (by 14% per second of swimming at max level). Modifier stops increasing if swimming duration exceeds 21 seconds.
        *   Grants `Slipping`: Increases movement speed in the rain (by 10% per second of movement at max level). Modifier stops increasing if duration exceeds 12.5 seconds.
        *   Grants `Gills`: Chance (45% at max level) to not consume an air unit while swimming or in other conditions.
    *   **`Phantom Boot`**: Grants `Phantom Bridge`: Creates temporary phantom blocks beneath the player's feet that any relic owner can walk on. Standing still for too long (6 seconds at max level) causes falling through until solid ground. Sneaking forces falling through.
    *   **`Springy Boot`**: Grants `Elasticity`: Increases block elasticity (by 100% at max level compared to slime blocks), enabling bouncing off them on landing. When activated on the ground, launches the player into the air.

### Charm Slot

![Charm Slot Icon](img/curios/charm_slot.png)

*   **Description:** A slot for small magical charms, often providing passive utility, protection, or specific conditional effects. The number of available Charm slots can be significantly increased by items like the `Leather Belt` (+8) and `Infinity Glove` (+1).
*   **Functionality:** Highly varied, ranging from environmental protection (fire, water breathing, falling), death prevention, mob interaction changes, to modifying L2Hostility mechanics. Some charms have limited charges and require recharging, while others are single-use.
*   **Compatibility:** Items tagged `#curios:charm` fit here. Many items tagged `#curios:hostility_curse` can also fit in this slot.
*   **Examples:**

    ![Various Charm Slot Items](img/curios/charm_slot_items.png)

    #### 1. Ars Additions
    *(Note: These charms have charges and can be recharged, in an Ars Nouveau Imbuement Chamber).*
    *   **`Charm of Emberward`**: Nullifies Fire Damage (walk through fire, swim in lava). Charges: 1000.
    *   **`Charm of Second Wind`**: Prevents death upon receiving fatal damage. Charges: 1.
    *   **`Charm of Unyielding Magic`**: Prevents beneficial effects from being dispelled. Charges: 3.
    *   **`Charm of Featherlight`**: Grants slow falling when falling more than 3 blocks. Charges: 20.
    *   **`Charm of Ocean's Breath`**: Enables breathing underwater (activates after air bubbles depleted). Charges: 1000.
    *   **`Charm of Ender Serenity`**: Prevents angering Endermen by looking at them. Charges: 100.
    *   **`Charm of Decay's End`**: Prevents being afflicted with the Wither effect. Charges: 10.
    *   **`Charm of Gilded Friendship`**: Makes Piglins and Piglin Brutes neutral, allowing safe interaction in Bastions. Charges: 1000.
    *   **`Charm of Darkvision`**: Grants Night Vision in low-light environments. Charges: 20.
    *   **`Charm of Snowstride`**: Enables walking on powdered snow without sinking. Charges: 1000.
    *   **`Resonant Shield`**: Protects from the Warden's sonic boom attack. *(Charges TBC)*.
    *   **`Void's Salvation`**: When falling into the void, teleports you to the last safe surface you were on. *(Charges TBC)*.

    #### 2. L2Hostility & L2Complements
    *(Note: Many L2Hostility items can often be worn in the Hostility Curse slot as well. Effects listed are when worn as Charm. Wearing as Curse might have additional effects or increased difficulty.)*
    *   **(L2Hostility) Looting Charms (`Unpolished`, `Magical`, `Chaotic`, `Miraculous`)**: Enables some hostility trait drops (check JEI for specifics for each tier).
    *   **(L2Hostility) `Curse of Envy`**: Get trait items when killing mobs with traits (2% chance per trait rank). Increases player difficulty by +50.
    *   **(L2Hostility) `Curse of Greed`**: Doubles (x2.0) hostility loot drop chance. Increases player difficulty by +50.
    *   **(L2Hostility) `Curse of Lust`**: Mobs you kill will drop all their equipped items. Increases player difficulty by +50.
    *   **(L2Hostility) `Curse of Wrath`**: Gain 1% attack damage per difficulty level difference against mobs with higher levels. Grants immunity to Blindness, Darkness, Mining Fatigue, Nausea, Slowness, Weakness. Increases player difficulty by +50.
    *   **(L2Hostility) `Curse of Sloth`**: Prevents gaining difficulty by killing mobs. Prevents mobs you kill from dropping hostility loot.
    *   **(L2Hostility) `Curse of Gluttony`**: Get `Bottle of Curse` when killing mobs with a level (2% chance per level).
    *   **(L2Hostility) `Pocket of Restoration`**: Automatically takes sealed items (like `Bottle of Curse`) placed inside, unseals them (applies the effect/curse), and returns the empty container.
    *   **(L2Complements) `Totem of Dream`**: When triggered (likely by fatal damage), returns the player to their home/spawn point, heals to full health, and becomes a `Fragile Warp Stone` to return to the death location. Valid against void damage. (Single use).
    *   **(L2Complements) `Totem of The Sea`**: Stackable (up to 16). Functions like a Totem of Undying, but can only be triggered when in water or rain. (Single use per totem).
    *   **(L2Complements) `Eternal Totem of Dream`**: Reusable version of the `Totem of Dream` with a 120-second cooldown.
    *   **Currently Unobtainable Items (L2Hostility):** *(Note: The following items require traits/materials that are currently disabled or unavailable for crafting in ATMA. This might change in future updates.)*
        *   `Curse of Pride`: Gain 1% health and 1% attack damage per difficulty level. Mob traits will be +100% more frequent.
        *   `Divinity Cross`: Prevents the Cleanse effect from clearing Level 1 beneficial effects.
        *   `Divinity Light`: Keeps your adaptive level at 0.
        *   `Platinum Star`: All melee damage bypasses damage cooldown. (Also fits in **Hands** slot).

    #### 3. Artifacts
    *Note: Artifacts share experience earned and level up through use.*

    *   **`Cloud in a Bottle`**: Grants `Air Jump`: Allows additional air jumps (up to 13 at max level).
    *   **`Obsidian Skull`**: Grants `Heat Resistance`: Completely absorbs damage from fire sources (up to 12 seconds at max level). If no fire damage is taken for 3 seconds, absorption time regenerates each second.
    *   **`Antidote Vessel`**:
        *   Grants `Poison Resistance`: Reduces the duration of negative effects received (by 80% at max level).
        *   Grants `Alchemical Touch`: Each successful attack steals duration (7.5 seconds at max level) from all positive effects on the target.
    *   **`Universal Attractor`**: Grants `Magnetism`: Toggleable ability with 3 modes: Attraction (Red - pulls items in 15 block radius), Repulsion (Blue - pushes items away), Neutrality (Purple - disables effect).
    *   **`Crystal Heart`**: Grants `Will to Live`: Increases the player's maximum health (by 18 points / 9 hearts at max level).
    *   **`Chorus Totem`**: Grants `Temporal Loop`: Each attack against the wearer has a chance per percent of missing health (7% at max level) to teleport the attacker to a random location within a radius (14 blocks at max level).
    *   **`Warp Drive`**: Grants `Translocation`: Teleports the player along their line of sight (up to 100 blocks at max level), then goes on cooldown (1 second at max level).

    #### 4. Glimmering Tales
    *   **`Charm of Strength`**: +50% Magic Damage.
    *   **`Charm of Capacity`**: +50% Max Mana.
    *   **`Charm of Regeneration`**: +50% Mana Regen.
    *   **`Charm of Nature`**: +10% Mana Regen.
    *   **`Charm of Earth`**: +10% Mana Regen, -20% Damage after Reduction (Reduces final damage taken).
    *   **`Charm of Life`**: +10% Mana Regen, +50% Regeneration Rate (Health).
    *   **`Charm of Flame`**: +100% Fire Damage, +100% Explosion Damage.
    *   **`Charm of Snow`**: -10% Damage after Reduction, +100% Freezing Damage.
    *   **`Charm of Ocean`**: +10% Mana Regen, +50% Magic Damage.
    *   **`Charm of Thunder`**: +20% Mana Regen, +100% Lightning Damage.

    #### 5. Nature's Aura
    *   **`Environmental Eye`**: *(Tooltip missing - Likely displays Aura levels in the surrounding environment).*
    *   **`Environmental Ocular`**: *(Tooltip missing - Likely an improved version of the Environmental Eye, perhaps with greater range or detail).*

    #### 6. Apotheosis
    *   **Potion Charms** (e.g., `Charm of Night Vision`, `Charm of Strength`, etc.): Crafted by combining a potion with Glowstone Dust and Echo Shards. Provides the corresponding potion effect passively while equipped (or in inventory if enabled). Effect duration matches the potion used.

    #### 7. The Twilight Forest
    *(Note: These charms are typically single-use and consumed upon activation).*

    *   **`Charm of Life I`**: Prevents death, consumed on use, grants short health regeneration. Found in loot chests.
    *   **`Charm of Life II`**: Prevents death, consumed on use, fully restores health, grants Regen IV, Resistance, and Fire Resistance for 30 seconds. Crafted from 4x Charm of Life I.
    *   **`Charm of Keeping I`**: Prevents loss of main hand, off-hand, and armor items on death. Consumed on use.
    *   **`Charm of Keeping II`**: Prevents loss of main hand, off-hand, armor, and hotbar items on death. Consumed on use.
    *   **`Charm of Keeping III`**: Prevents loss of all inventory items on death. Consumed on use.

    #### 8. Relics (Reliquified)
    *Note: Relics share experience earned and level up through use.*

    *   **`Spore Sack`**: Grants `Spore Mist`: When health drops below 50%, releases homing spores (up to 20). Spores deal damage equal to % missing health (75% at max level) and block healing for 5s. Can trigger again once health rises above 50%.
    *   **`Shadow Glaive` (Combined Relic)**:
        *   Grants `Mayhem`: Dealing damage has a chance (25%) to trigger a projectile that bounces chaotically between nearby targets (within 16 blocks) up to 10 times, dealing % of trigger damage (50%).
        *   Grants `Cloning`: Each projectile bounce from `Mayhem` has a chance (20%) to spawn an additional identical projectile.

    #### 9. Reliquified Ars Nouveau
    *Note: Relics share experience earned and level up through use.*

    *   **`Quantum Bubble`**: Grants `Quantification`: When an enemy projectile appears within 2 blocks, activates an aura (up to 16s) that halts and traps hostile projectiles in bubbles for 8s. Goes on cooldown (13s) after aura expires.
    *   **`Emblem of Defense`**: Grants `Defense`: Automatically applies a linked spell (max 10 components, must start with 'Touch') to an enemy attacking the player, then goes on cooldown (10s). Requires inscribing spell via Scribe's Table.
    *   **`Emblem of Assault`**: Grants `Assault`: Automatically applies a linked spell (max 10 components, must start with 'Touch') to the attacked target, then goes on cooldown (15s). Requires inscribing spell via Scribe's Table.

    #### 10. Reliquified Twilight Forest
    *Note: Relics share experience earned and level up through use.*

    *   **`Cicada in a Bottle`**: Grants `Cicada's Curse`: Chance on hit (70% at max level) to inflict Cicada's Curse on the target for 12s, forcing nearby mobs to attack that target.
    *   **`Firefly Queen`**: Grants `Glowkeeper`: Generates firefly larva in an internal buffer (max 8) every 2s. When in complete darkness, consumes 1 larva to place a temporary firefly nearby for light.
    *   **`Twilight Feather`**: Grants `Execution`: When attacking a target whose health doesn't exceed % of player's max health (5% at max level), chance to instantly execute it, transforming it into a small bird.
    *   **`Bottle of Maple Syrup`**: Grants `Sugar Rush`: Eating a waffle increases health regen (by 200%) for 20s (effect stacks). Chance (75%) the waffle won't be consumed.

### Talent Slot

![Talent Slot Icon](img/curios/talent_slot.png) or ![Talent Slot Icon 2](img/curios/talent_slot_2.png)

*   **Description:** A slot seemingly intended for specialized items that grant or modify abilities, often related to specific spells or mechanics from particular mods. In ATMA, this slot is primarily utilized by the **Traveloptics** addon for **Iron's Spells 'n Spellbooks**.
*   **Functionality:** Items in this slot typically alter how specific spells function or provide passive benefits related to certain spell schools or actions. Many items that fit here can also fit into other slots (Ring, Necklace, Bracelet), providing flexibility.
*   **Compatibility:** Items tagged `#curios:talent` fit here.
*   **Examples:**

    ![Various Talent Slot Items](img/curios/talent_slot_items.png)

    #### 1. Iron's Spells 'n Spellbooks (Addon: Traveloptics)
    *(Note: These items often fit multiple slots. The descriptions below apply regardless of which compatible slot they are equipped in, unless stated otherwise.)*
    *   **`Aetherial Despair Ring`**: Axe Blades of Despair spell gain vertical trajectory and move 50% faster. (Also fits **Ring** slot).
    *   **`Firestorm Ring`**: Transforms meteors from Meteor Storm spell into exploding flare bombs with flame jets. Spell can no longer directly target entities. (Also fits **Ring** slot).
    *   **`Azure Ignition Bracelet`**: Permanently ignites Ignis-themed spells with soul fire, increasing their damage. (Also fits **Bracelet** slot).
    *   **`Nightstalker's Band`**: Allows the `Reversal` spell to be cast without a weapon. Reflecting a projectile grants the `Assassin` effect for 5 seconds (boosts movement speed and greatly enhances attack damage). Effect ends upon striking an entity. (Also fits **Bracelet** slot).
    *   **`Energy Unbound Necklace`**: Grants the caster freedom to look around while casting Death Laser and allows movement at 80% reduced speed. However, the laser's damage is reduced by 20%. (Also fits **Necklace** slot).
    *   **`Sigil of the Spider Sorcerer`**: Aspect of the Spider spell now allows wall climbing. Casting Aspect of the Spider and striking an enemy grants a 50% chance to poison them for 3 seconds. (Also fits **Necklace** slot).
    *   **`Amulet of Spectral Shift`**: Spectral Blink spell now teleports the targeted entity to *your* location while crouching. (Also fits **Necklace** slot).

### Spell Book Slot

![Spell Book Slot Icon](img/curios/spell_book_slot.png)

*   **Description:** A dedicated slot introduced by **Iron's Spells 'n Spellbooks** specifically for holding Spell Books. Equipping a Spell Book here allows the player to access and cast the spells inscribed within it using the spell selection and casting keybinds (default 'C' and 'V').
*   **Functionality:** Primarily serves as the container for learned spells. Additionally, equipped Spell Books often provide passive statistical bonuses, such as increased Max Mana, Cooldown Reduction, Cast Time Reduction, or bonuses to specific spell schools (e.g., Fire Spell Power). The number of spells a book can hold varies by tier and type.
*   **Compatibility:** Items tagged `#curios:spellbook` fit here. This includes books from Iron's Spells 'n Spellbooks and its various addons, as well as All the Wizard Gear.
*   **Examples:**

    ![Various Spell Book Slot Items](img/curios/spell_book_slot_items.png)

    #### 1. Iron's Spells 'n Spellbooks (Base Mod)
    *   **Tiered Spell Books:**
        *   `Flimsy Journal` (Copper): 5 Spell Slots.
        *   `Ironbound Tome` (Iron): 6 Spell Slots.
        *   `Apprentice's Spell Book` (Gold): 8 Slots, +15% Cast Time Reduction, +50 Max Mana.
        *   `Enchanted Spell Book` (Diamond): 10 Slots, +100 Max Mana.
        *   `Ancient Codex` (Netherite): 12 Slots, +20% Cooldown Reduction, +200 Max Mana.
    *   **Special/Loot Spell Books:**
        *   `Rotten Spell Book`: 8 Slots, **-15% Spell Resistance**, +100 Max Mana.
        *   `Blaze Instruction Manual`: 10 Slots, +10% Fire Spell Power, +200 Max Mana.
        *   `Cursed Doll`: 10 Slots, +1 level to Blood Needles & Acupuncture, +10% Blood Spell Power, +10% Spell Resistance, +200 Max Mana.
        *   `Druidic Tome`: 10 Slots, +10% Nature Spell Power, +200 Max Mana.
        *   `Dragonskin Spell Book`: 12 Slots, +10% Ender Spell Power, +200 Max Mana.
        *   `Villager Bible`: 10 Slots, +8% Holy Spell Power, +8% Cast Time Reduction, +200 Max Mana.
    *   **Unique Spell Books (Often contain pre-inscribed spells):**
        *   `Grimoire of Evokation`: 10 Slots, +10% Evocation Spell Power, +200 Max Mana. (Contains Evoker spells).
        *   `Necronomicon`: 10 Slots, +2 levels to Raise Dead, +200 Max Mana. (Contains Blood/Undead spells).

    #### 2. All the Wizard Gear
    *   `Allthemodium Spell Book`: 13 Slots, +30% Cooldown Reduction, +15% Cast Time Reduction, +300 Max Mana.
    *   `Vibranium Spell Book`: 14 Slots, +40% Cooldown Reduction, +25% Cast Time Reduction, +300 Max Mana.
    *   `Unobtainium Spell Book`: 15 Slots, +50% Cooldown Reduction, +35% Cast Time Reduction, +300 Max Mana.

    #### 3. Traveloptics
    *   `Shellbound`: 12 Slots, +200 Max Mana, +10% Nature Spell Power, +10% Cooldown Reduction.
    *   **Unique Spell Books:**
        *   `Chronicles Of The Firelord`: 12 Slots, +1 level to Burning Judgment, +300 Max Mana, +15% Fire Spell Power, +15% Eldritch Spell Power. (Contains Fire spells).
        *   `The Accused Codex`: 12 Slots, +300 Max Mana, +10% Cooldown Reduction, +20% Ice Spell Power. (Contains Ice spells).
        *   `Archive Of Abyssal Secrets`: 12 Slots, +1 level to Cursed Minefield, +300 Max Mana, +15% Ender Spell Power, +15% Eldritch Spell Power. (Contains Ender/Void spells).

    #### 4. Cataclysm Spellbooks
    *   `Codex of Malice`: 12 Slots, +300 Max Mana, +30% Ice Spell Power.
    *   `Ignis Spellbook`: 12 Slots, +30% Fire Spell Power, +300 Max Mana.
    *   `Book o' R'lyeh`: 12 Slots, +30% Abyssal Spell Power, +300 Max Mana.
    *   **Unique Spell Books:**
        *   `Desert Spellbook`: 10 Slots, +200 Max Mana, +20% Nature Spell Power, +10% Holy Spell Power. (Contains Nature/Sand spells).

    #### 5. GameTechBC's Spellbooks
    *   **Unique Spell Books:**
        *   `GTBC's Magical Repository`: 10 Slots, +200 Max Mana, +15% Spell Power, +10% Cooldown Reduction. (Contains custom spells).


### Bundle Slot

![Bundle Slot Icon](img/curios/bundle_slot.png)

*   **Description:** A slot designed to hold pouch-like items that offer portable storage, similar to the vanilla Bundle concept but integrated with Curios.
*   **Functionality:** Provides extra inventory space accessible via a keybind while the item is equipped in this slot (or held in the hotbar).
*   **Compatibility:** Items tagged `#curios:bundle` fit here.
*   **Examples:**

    ![Various Bundle Slot Items](img/curios/bundle_slot_items.png)

    #### 1. Ars Elemental
    *   **`Trinkets Pouch`**: A magical pouch crafted from Magebloom Fiber used to store items and reduce inventory clutter. Can be opened with the 'J' key (configurable) while equipped in a Curios slot or held in the hotbar.
    *   **`Spellcaster Bag`**: An upgraded, larger version of the Trinkets Pouch. Can also be opened with the 'J' key and can be dyed different colors.

### Heart Amulet Slot

![Heart Amulet Slot Icon](img/curios/heart_amulet_slot.png)

*   **Description:** A dedicated slot added by **Baubley Heart Canisters** specifically for the `Heart Amulet` and its variants.
*   **Functionality:** When equipped, these amulets allow the player to store various types of Heart Canisters (Red, Orange, Yellow, Green, Blue) or potentially interact with other health-related mechanics. Each canister stored typically increases the player's maximum health. The amulet itself can be opened (++rbutton++) to manage its contents.
*   **Compatibility:** Items tagged `#curios:heart_amulet` fit here.
*   **Examples:**

    ![Heart Amulet Items](img/curios/bhc_amulets.png)

    #### 1. Baubley Heart Canisters
    *   **`Heart Amulet`**: The primary item for this slot. Acts as a container for Heart Canisters, which increase maximum health when socketed. Right-click the amulet in your inventory or Curios slot to open its interface and add/remove canisters. *(Refer to Baubley Heart Canisters guide - WIP for canister details)*.
    *   **`Soul Amulet`**: An upgraded amulet for this slot. It can also be opened via right-click.

---

## Other Artifacts & Relics (Non-Curios)

These items from the Artifacts and Relics mods provide effects but are typically held or used directly, rather than equipped in a dedicated Curios slot. Some might have alternative equip slots (like the Umbrella potentially fitting 'Back'), but their primary function often involves holding them.

![Other Artifacts & Relics](img/curios/other_artifacts.png)

### 1. Relics
*Note: Relics share experience earned and level up through use.*

*   **`Infinite Ham` (Combined Relic)**: *(Held food item)*
    *   Grants `Regeneration`: Every 10 seconds (at max level), regenerates up to 6 edible chunks, each restoring 13 hunger points. When consumed, the relic automatically uses the required number of chunks to replenish the player's hunger. (Note: Does not improve max health).
    *   Grants `Marinade`: Allows applying potion effects to the relic by left-clicking it with a potion in the inventory. Each time the relic is consumed, it applies these effects to the player for 9 seconds per hunger point restored. Using a water bottle clears the last applied potion effect.
    *   Grants `Meat Bat`: Allows the relic to be used as a melee weapon, dealing 7 damage and stunning the target for 0.5 seconds per chunk. Consumes all chunks when attacking, regardless of the target's remaining health.
*   **`Space Dissector`**: *(Held item)*
    *   Grants `Dissection`: Holding RMB creates a portal at a point along the line of sight. Releasing RMB within a distance of 112 blocks creates a second portal, linking it to the first. When a living entity approaches a portal, it is teleported to the linked portal. Portals do not function if impassable blocks are in their way. After 60 seconds, the portals close and disappear.
*   **`Magic Mirror`**: *(Held item)*
    *   Grants `Wormhole`: Upon use, teleports the owner to their spawn point if it is within 6000 blocks, then goes on cooldown for 30 seconds.
*   **`Blazing Flask`**: *(Held item)*
    *   Grants `Eternal fire`: Using the ability on a block creates a restricted flight zone with a maximum flight speed of 8 blocks per second and a height of 15 blocks. The area size depends on the amount of fire within a radius of 5 blocks around the center, but if there is no fire at all, the zone will not be created.

### 2. Artifacts
*Note: Artifacts share experience earned and level up through use.*

*   **`Everlasting Beef`**: *(Food item)* Food item that is not consumed upon eating. Restores a small amount of hunger and saturation.
*   **`Eternal Steak`**: *(Food item)* Food item that is not consumed upon eating. Restores more hunger and saturation than Everlasting Beef.
*   **`Umbrella`**: *(Held item - might also fit Back slot)*
    *   Grants `Soft Fall`: When held, reduces the player's vertical speed, negating fall damage.
    *   Grants `Glide` (Push): Pressing LMB while gliding propels the player backward and triggers a cooldown of 0.5 seconds. The push can be used up to 13 times in succession before the player touches the ground.
    *   Grants `Air Shield`: When used (likely via blocking/RMB), functions as a shield, pushing targets up to 6 blocks away (at max level).

---

## How to Equip Curios Items

1.  Press the **Curios key** (Default key: 'G') to open the Curios slots GUI.
2.  Identify the appropriate slot type for the item you want to equip (e.g., Head, Back, Necklace, Hands, Belt, Charm, Ring, Focus).
3.  Drag the desired Curios item from your main inventory into a compatible empty slot in the Curios GUI.
4.  The item is now equipped, and its effects (if any) should be active!

---

> **Curios API** | [CurseForge Link](https://www.curseforge.com/minecraft/mc-mods/curios)
