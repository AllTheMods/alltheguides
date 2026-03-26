# Botania Mana Enchanter

**Botania Mana Enchanter** is a structure added by **Botania**. It uses **Mana** provided with **Sparks** or **Mana Spreaders** to enchant equipment with enchantments defined by **Enchanted Books** dropped nearby, _without consuming the books._ This is the slowest, yet only way to automate the process of duplicating and enchanting books using the applicator.

## Building Enchanter

**Botania Mana Enchanter** and **Enchantment Applicator** can both be automated with the required materials.

**Materials**

* 3 Routers
* 3 Activator Modules
* 1 Wand of the Forest

***

* 17 Obsidian
* 1 Lapis Block
* 1 Mana spark
* 6 Mana Pylons
* 10 Dirt/Grass blocks
* 10 Mystical Flowers

***

* 1 Cyclic Dropper
* 3 Building blocks
* 1 Cyclic Item detector
* 2 Redstone
* 1 Redstone Torch
* 1 RFtools Timer
* 1 Vacuumulator

***

* 5 Pipez (+1 upgrade for filtering)
* Black hole Tank
* Enchantment Applicator
* Disenchanter
* Entangled Block
* Trash can

Build the **Multi-Block** structure shown below. **Botania Lexica** will help visually seeing block positions, then place down 3 **Modular Routers** facing into the **Mana Enchanter**, as shown below.

![](../../.gitbook/assets/kPa02o1.png)

## Routers Configuration

**Activator Module** for ALL 3 routers should look like this. Set the **FRONT** face direction (middle part of GUI) as shown below.

![](../../.gitbook/assets/1MTtkbM.png)

{% tabs %}
{% tab title="Left Router" %}
Tool/Weapon input, keep this fed with new tools or weapons. (Ex: RS with crafting card). Be sure this is always full with a tool and set it to Pulse

![](../../.gitbook/assets/1voCURd.png)
{% endtab %}

{% tab title="Top Router" %}
Tool/Weapon Output. Be sure to set this to Redstone Mode: High

![](../../.gitbook/assets/Xfo3D4W.png)
{% endtab %}

{% tab title="Right Router" %}
**Wand Of The Forest**. Give it speed upgrades if possible and a wand of the forest and set it to always on, this router always tries to start an enchanting process

![](../../.gitbook/assets/blkUApI.png)
{% endtab %}
{% endtabs %}

## Automation Setup

Place a **Cyclic Dropper** 1 block away from the **Enchanter** and set to **Always Active**. Place an **Item Detector** ontop of the bottom left flower, and a redstone line on the **LEFT** router

![](../../.gitbook/assets/xnHDMnN.png)

{% hint style="info" %}
The Dropper will drop an enchanted book triggering the **Item detector**, which triggers the **LEFT** router, which then puts 1 tool into the **Enchanter**. The **RIGHT** Router (with the **Wand of the Forest**) will initiate the enchanting process.
{% endhint %}

* Place 3 blocks (as shown below)
* Redstone Torch on the **TOP** router (against left block)
* **RFTools Timer** (100 Delay, with “Pause while redstone is active” enabled) on 3rd block facing right
* **Vacuumulator** with redstone on top (Set **Redstone Control** HIGH).

![](../../.gitbook/assets/BJ03fS6.png)

Setup pipes to pull out from the **TOP** router (Enchanted Tool), and the **Vacuumulator** (Enchanted Book).

![](../../.gitbook/assets/fqjil6M.png)

Pipes will then go into the **Enchantment Applicator**. **Black Hole Supreme Tank** on top of the **Enchantment Applicator**.

![](../../.gitbook/assets/kVz4z9V.png)

{% hint style="info" %}
Enchanting higher levels will take more than 64 buckets (internal applicator buffer) of XP/Essence, which a **Black Hole Tank** will be required on top of the applicator to act as a secondary buffer. **Liquid XP** will work up too _level 20_, afterwards **Mob Essence** will be required. The [Applicator](../../mods/enchantment-applicator.md) page will explain best methods of generating XP or Mob Essence.
{% endhint %}

Pipe the new combined Tool out of the **Applicator** and put it into a **Cylic Disenchanter** to split the 2 again

![](../../.gitbook/assets/r2Kgd5c.png)

Add a pipe, an **Entangled block** (linked to the **Dropper** at the beginning) and a **Trashcan**. Now set filters in your Pipez extraction point together with a destination tool. This makes the Book go in a loop and come back to the start of the cycle

![](../../.gitbook/assets/7chMmZ3.png)

Rightclick the side of the Entangled block which has the pipe leading into it with the destination tool, add the Book to the filter and remove the NBT tag so all books go to the dropper

![](../../.gitbook/assets/a1mMl4Q.png)

Do the same with your pickaxe, remove the NBT data, so all (old) tools go to the bin

![](../../.gitbook/assets/y7r4ST2.png)

That should look something like this

![](../../.gitbook/assets/OiqfDAf.png)

Dont forget to put a spark on your Mana Enchanter and get a decent Mana Supply! Put a book into the dropper and the whole process should work automaticly.

![](../../.gitbook/assets/pwTzGmX.png)

> Botania | [CurseForge](https://legacy.curseforge.com/minecraft/mc-mods/botania)
