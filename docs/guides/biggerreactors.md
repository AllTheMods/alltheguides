---
title: Bigger Reactors
---

# Bigger Reactors

**Reactors** are the primary multi-block of **Bigger Reactors**. Loosely inspired by the real-life RBMK design, reactors may be used as either a power generator (in **Passive** mode) or as a heat source (in **Active** mode). Reactors consume and produce various Fuel and Waste products, and are highly customizable.

As of **Bigger Reactors** 0.5.2, the smallest possible reactor size is **3 × 3 × 3**. With the default config, reactors may be built as large as **128 × 128 × 192**, however this may be changed to an absolute maximum of **192 × 192 × 256**.

## Components

### Required

The following components are the bare minimum required to construct any type of reactor.

- **Reactor Terminals**: are the heart of your reactor. 
- **Reactor Casings**: make up the frame and walls of your reactor.
- **Fuel Rods**: are where Fuel and Waste are contained.
- **Control Rods**: are used to maintain control over the reaction.
- **Access Ports**: are used to insert Fuel and extract Waste.

### Type-Specific

Certain components may only be used with a specific type of reactor, and cannot be used together in the same reactor.

The first type of reactor are **Passive Reactors**. These output the energy they generate directly as RF, which may be used by other machines.

- **Power Taps** are where you extract power from a passive reactor.
: The second type of reactor are **Active Reactors**. These convert the energy they generate into heat, which is used to heat up fluids.
- **Coolant Ports** are used to insert “cold” fluids (such as water) and extract “hot” fluids (such as steam).
- **Coolant Manifolds** are used to increase the surface area for heat transfer.

### Optional

Some components are entirely optional and are not required to build a functioning reactor. These may, however, allow for automation and remote control of reactors.

- **Redstone Ports** allow for control of various reactor functions via Redstone circuits.
- **Computer Ports** allow for control of various reactor functions via Lua scripting. This requires a computers mod such as CC: Tweaked to be installed.
- **Reactor Glass** functions identically to casings, but may only be used on walls. It allows you to see inside of the reactor.

## Moderators

**Reactor Moderators** (_commonly incorrectly referred to as **Reactor Coolants**_) are materials placed inside of a Reactor during construction. When a reactor is in operation, a moderator may change the way the reactor performs depending its properties.

**Moderators** have four main properties that affect the reactor simulation:

- **Absorption**: The speed at which radiation is absorbed and converted to case heat.
- **Efficiency**: How efficiently absorbed radiation is converted into heat.
- **Moderation**: The effectiveness at which radiation is moderated ("softened").
- **Conductivity**: How well heat is transferred from the fuel rods to the reactor casing.

In general, higher values are always better (except for absorption, which may be better or worse depending on your reactor design). For a more in-depth explanation on how to use the information here, see the [simulation page](https://biggerseries.net/en/biggerreactors/reactor/simulation).

Something to note is that Modpack authors have the ability to add or modify moderators. For an accurate list of supported blocks/fluids, use [Just Enough Items (JEI)](https://www.curseforge.com/minecraft/mc-mods/jei) by checking the uses for the Reactor Terminal (**currently broken on multiplayer**).

??? "Moderator Properties"
    _The values listed below are accurate for Bigger Reactors 0.5.2, for Minecraft 1.16.5. Also correct for 0.6.x (1.17-1.19)_

    | ID | Absorption | Efficiency | Moderation | Conductivity |
    | -- | ---------- | ---------- | ---------- | ------------ |
    | astralsorcery:liquid_starlight | 0.85 | 0.8 | 2.0 | 3.0
    | biggerreactors:ludicrite_block | 0.6 | 0.87 | 3 | 3
    | bloodmagic:life_essence_block | 0.7 | 0.55 | 1.75 | 2.5
    | mekanism:ethene | 0.37 | 0.65 | 1.9 | 1.5
    | mekanism:hydrofluoric_acid | 0.6 | 0.45 | 1.4 | 2.5
    | mekanism:hydrogen | 0.2 | 0.3 | 1.2 | 0.1
    | mekanism:hydrogen_chloride | 0.31 | 0.65 | 1.7 | 1
    | mekanism:lithium | 0.7 | 0.6 | 1.04 | 0.7
    | mekanism:oxygen | 0.01 | 0.35 | 1.04 | 0.1
    | mekanism:sodium | 0.23 | 0.6 | 1.7 | 1
    | mekanism:steam | 0.33 | 0.5 | 1.33 | 0.5
    | mekanismgenerators:deuterium | 0.03 | 0.3 | 1.07 | 0.1
    | minecraft:air | 0.1 | 0.25 | 1.1 | 0.05
    | minecraft:cave_air | 0.1 | 0.25 | 1.1 | 0.05
    | minecraft:glass | 0.2 | 0.25 | 1.1 | 0.3
    | minecraft:ice | 0.33 | 0.33 | 1.15 | 0.1
    | minecraft:snow_block | 0.15 | 0.33 | 1.05 | 0.05
    | minecraft:void_air | 0.1 | 0.25 | 1.1 | 0.05
    | minecraft:water | 0.33 | 0.5 | 1.33 | 0.1
    | minecraft:lava | 0.33 | 0.33 | 1.15 | 0.7
    | forge:storage_blocks/allthemodium | 0.66 | 0.9 | 3.5 | 3.5
    | forge:storage_blocks/aluminum | 0.5 | 0.78 | 1.42 | 0.6
    | forge:storage_blocks/bronze | 0.51 | 0.77 | 1.41 | 1
    | forge:storage_blocks/copper | 0.5 | 0.75 | 1.4 | 1
    | forge:storage_blocks/diamond | 0.55 | 0.85 | 1.5 | 3
    | forge:storage_blocks/electrum | 0.53 | 0.82 | 1.47 | 2.2
    | forge:storage_blocks/emerald | 0.55 | 0.85 | 1.5 | 2.5
    | forge:storage_blocks/enderium | 0.53 | 0.88 | 1.6 | 3
    | forge:storage_blocks/gold | 0.52 | 0.8 | 1.45 | 2
    | forge:storage_blocks/graphite | 0.1 | 0.5 | 2 | 2
    | forge:storage_blocks/invar | 0.5 | 0.79 | 1.43 | 0.6
    | forge:storage_blocks/iron | 0.5 | 0.75 | 1.4 | 0.6
    | forge:storage_blocks/lead | 0.75 | 0.75 | 1.75 | 1.5
    | forge:storage_blocks/lumium | 0.75 | 0.55 | 1.5 | 1.8
    | forge:storage_blocks/nickel | 0.5 | 0.82 | 1.46 | 0.6
    | forge:storage_blocks/osmium | 0.51 | 0.77 | 1.41 | 1
    | forge:storage_blocks/platinum | 0.53 | 0.86 | 1.58 | 2.5
    | forge:storage_blocks/signalum | 0.63 | 0.66 | 1.5 | 1.8
    | forge:storage_blocks/silver | 0.51 | 0.79 | 1.43 | 1.5
    | forge:storage_blocks/steel | 0.5 | 0.78 | 1.42 | 0.6
    | forge:storage_blocks/tin | 0.3 | 0.7 | 1.35 | 0.75
    | forge:storage_blocks/unobtainium | 0.95 | 0.82 | 2 | 5
    | forge:storage_blocks/vibranium | 0.15 | 0.75 | 8 | 4
    | forge:storage_blocks/zinc | 0.51 | 0.77 | 1.41 | 1
    | biggerreactors:liquid_obsidian | 0.3 | 0.7 | 1.35 | 0.75
    | allthemodium:molten_allthemodium | 0.66 | 0.9 | 3.5 | 3.5
    | allthemodium:molten_vibranium | 0.15 | 0.75 | 8 | 4
    | allthemodium:molten_unobtainium | 0.95 | 0.82 | 2 | 5
    | allthemodium:vapor_allthemodium | 0.66 | 0.9 | 3.5 | 3.5
    | allthemodium:vapor_vibranium | 0.15 | 0.75 | 8 | 4
    | allthemodium:vapor_unobtainium | 0.95 | 0.82 | 2 | 5
    | forge:superheated_sodium | 0.23 | 0.6 | 1.7 | 1
    | forge:redstone | 0.75 | 0.55 | 1.6 | 2.5
    | forge:ender | 0.9 | 0.75 | 2.0 | 2

> Bigger Reactors | [CurseForge](https://legacy.curseforge.com/minecraft/mc-mods/biggerreactors)