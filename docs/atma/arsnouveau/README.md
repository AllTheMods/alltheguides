---
title: Ars Nouveau
description: A Guide for Ars Nouveau in All the Magic - Arcana
authors:
 - Xannaeh
---

# Ars Nouveau



### Spell Focus

Ars Nouveau is a magic mod that integrates heavily with Curios, allowing its Spell Focus to be equipped in the curios slot `Spell Focus` ![Spell Focus Slot](../img/arsnouveau/spell_focus_slot.png).
Equipping a Focus provides passive benefits and enhances certain spells or schools of magic.
Anything explicitly tagged as `#curios:an_focus` can go in this slot.

![Spell Focus Items](../img/arsnouveau/spell_focus_items.png)

#### Common Mechanics for Elemental Focus (Earth, Water, Fire, Air)

*   **Attunement:** Each elemental focus is attuned to a specific school of magic (e.g., Focus of Earth -> Earth School).
*   **Amplification & Discount:** While equipped, spells (glyphs) belonging to the attuned school are generally stronger and/or cost less mana.
*   **Lesser Focus Drawback:** The basic ("Lesser") version of these elemental Focus often weakens spells from the *other* three elemental schools (Fire, Water, Earth, Air).
*   **Major Focus Bonus:** An upgraded version typically provides an additional, more powerful bonus under specific conditions, likely alongside the amplification/discount.

#### Specific Spell Focus Details

 1. Focus of Earth

*   **Attunement:** Earth
*   **Lesser Drawback:** Weakens Fire, Water, Air glyphs.
*   **Major Bonus:** Grants Mana Regen I while the wearer is below Y=0 (deep underground).
*   **Empowered Effects:**
    *   `Poison Spores` / `Grow`: Deals damage to Undead mobs, chance to spawn a `Spore Blossom`.
    *   `Gravity` (Augmented with `Sensitive`): Creates a gravity well pulling entities towards the center (filter-compatible).
    *   Passively grants Knockback Resistance.
    *   Boosts natural and instant Healing effects received by 1.5x.

 2. Focus of Water

*   **Attunement:** Water
*   **Lesser Drawback:** Weakens Fire, Earth, Air glyphs.
*   **Major Bonus:** Grants Mana Regen I while wet; OR Mana Regen II + Dolphin's Grace effect while swimming.
*   **Empowered Effects:**
    *   `Freeze`: Applies stacking "Freezing" buildup, eventually inflicting "Frozen" status (short duration, stops healing).
    *   `Freeze` (Used after `Conjure Water`): Turns the conjured water into Ice blocks.
    *   `Summon Steed`: Summons a rideable Dolphin instead (build speed by timing jumps out of water).
    *   Converts Drowning damage dealt *to* water creatures into Magic damage.

 3. Focus of Fire

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

 4. Focus of Air

*   **Attunement:** Air
*   **Lesser Drawback:** Weakens Fire, Water, Earth glyphs.
*   **Major Bonus:** Grants Mana Regen I while the wearer is above Y=200 OR while under the "Shocked" effect.
*   **Empowered Effects:**
    *   `Launch` (Augmented with `Extend Time`): Applies the `Levitate` effect instead of just launching.
    *   `Cut`: Gives a chance to drop a mob's head or skull if `Cut` deals the killing blow.

 5. Focus of Necromancy

*   **Mechanics:** Does not follow standard elemental attunement/drawback rules.
*   **Effects:**
    *   Summoned Wolves, Undead, and Vexes will revive once upon death if the summoner is wearing the focus, returning with "blood lust".
    *   Summoned undead specifically will cast Homing spells when you do.
    *   Summoned undead specifically will heal you each time they kill an enemy.

 6. Focus of Summoning

*   **Mechanics:** Does not follow standard elemental attunement/drawback rules. Special focus for enhancing summons.
*   **Effects:**
    *   Grants summons (from spells) additional duration, strength, and speed.
    *   Deals damage to enemies that kill your summons (similar to Thorns for summons).
    *   Casting spells that target you (like `Self` or `Orbit` casting methods) will also cast a copy on your nearby summons.

 7. Focus of Block Shaping

*   **Mechanics:** Does not follow standard elemental attunement/drawback rules. Special focus for block manipulation spells.
*   **Effects:**
    *   **Impact Damage:** Blocks moved by spells (`Launch`, `Gravity`, `Pull`, `Knockback`, etc.) now deal damage to entities they collide with. Damage scales with your Spell Damage stat, the block's hardness, and the block's speed.
    *   **Spell Continuation:** Modifying, creating, or moving a block causes the remainder of the spell sequence to target the new or moving block, rather than the original target point.
        *   *Example (Creation):* `Freeze` -> `Break` will now correctly target the newly formed ice block with `Break`.
        *   *Example (Movement):* `Conjure Mageblock` -> `Launch` -> `Ignite` will launch the block, and the `Ignite` effect will apply to the moving block.
    *   Affects glyphs like `Conjure Mageblock`, `Freeze`, `Break`, `Exchange`, `Place Block`, `Launch`, `Pull`, etc.
    *   Synergizes heavily with `Area of Effect` (AoE) augmentation to manipulate or weaponize many blocks simultaneously.

 8. Focus of Transmutation from *Ars Technica*

*   **Mechanics:** Does not follow standard elemental attunement/drawback rules. Focus for item processing and enhancement glyphs.
*   **Core Function:** Augments spells with the `Luck` effect and improves specific processing glyphs.
*   **Provides the following bonuses:**
    *   2x Speed: For `Press`, `Polish`, and `Whirl` glyphs.
    *   2x Items Processed: For `Press` and `Polish` glyphs (processes two items per operation).
    *   2x Chance-Based Outputs: For `Obliterate` and `Whirl` glyphs (e.g., doubling ore dust chance).
    *   2x Damage: For the `Obliterate` glyph.


*Sources used for this guide include the [ars guide](https://ars.guide/docs/drygmy/guide/) and [ars wiki](https://www.arsnouveau.wiki/category/automation/entry/drygmy_charm/).*

> Ars Nouveau | [CurseForge](https://www.curseforge.com/minecraft/mc-mods/ars-nouveau) | [Ars Guide](https://ars.guide/) | [Wiki](https://www.arsnouveau.wiki/)
