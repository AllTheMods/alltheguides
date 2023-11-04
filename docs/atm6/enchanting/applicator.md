---
title: Enchantment Applicator
authors:
    - Seg
---

# Enchantment Applicator

**Enchantment Applicator** is a machine in **Industrial Foregoing**. It's used to apply enchantments like an anvil, however it can also grant an additional enchantment level when combining the _same enchantment level_ of an **Item** and an **Enchantment Book**, ignoring enchantment levels to reach a max of level 255 (**CCLV**)!. 


This process will require a **Black Hole Tank** (_Preferably **Supreme**_), and **Liquid XP** or **Mob Essence** inside the tank on top of the applicator to function properly. Using **Liquid XP** will only increase enchantment level up to 20 (**XX**), afterwards will require **Mob Essence**.

After gaining an additional enchantment level, you'll want to duplicate the enchant. There's 2 known ways,

## Duplicating Enchants

- Disenchant and use [Botania Mana Enchanter](botania.md) to duplicate enchantment books on a new **Item**.
- Duplicate **Item** using [Mahou Projection](mahou.md). (_Only works with certain tools, **NOT ARMOR**_).
    - _Armor enchants can be forced on tools using **Pedestal Anvil**_


!!! Warning "Using the same **Item** in applicator will increase **Repair Costs**, making combining enchants more expensive!"

## Making Essence

### Converting Liquid XP

**XP Liquid** can be converted to **Mob Essence** using **PneumaticCraft** Aeriel Interface.

- Craft a **Dispenser Upgrade**, and placed inside **Aerial Interface**.
- Change **Dispesser Upgrade** configuration for **Mob Essence**.
- Apply 15 Bars of pressure to **Aerial Interface**.
- Pump **XP Liquid** in -> output **Mob Essence**

### Converting XP Orbs

**XP Orbs** can be converted to **Mob Essence** using **Modular Routers**. Any best way you can generate and feed Modular Router XP Orbs, but be careful that **XP Clumps** can cause issues.

One way this can be done is growing **Mystical Agriculture** experience essence.

You will need,

- RFTools Craft (Crafts Essence into Experience Droplets)
- A Modular Router
- 9 Speed Upgrades
- Activator Module (For **Modular Router** to consume and spit out **XP Orbs**)
- Vacuum Module (To Collect **XP Orbs**)
- XP Vacuum Augment (Placed inside **Vacuum Module**, convert to convert **XP Orbs** into **Mob Essence**)
- Fast Pickup Augment (Placed inside **Vacuum Module** to make **Vacuum Module** collect faster)

: **Module Router** will consume given experience droplets and spit out **XP Orbs**. **Vacuum module** will collect the **XP Orbs** from configured face(s). **XP Vacuum Augment** will convert the consumed XP into **Mob Essence**, which will then be automatically outputted to a tank configured face of the Modular Router. 

### Woot

Using **Woot**, you can install the **Summit** perk. This will output **Mob Essence** through **Fluid Output** each operation (simulated mob death). The best mob to use one that has the most **HP**.