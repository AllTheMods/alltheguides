# Bigger Reactors

**Reactors** are the primary multi-block of **Bigger Reactors**. Loosely inspired by the real-life RBMK design, reactors may be used as either a power generator (in **Passive** mode) or as a heat source (in **Active** mode). Reactors consume and produce various Fuel and Waste products, and are highly customizable.

As of **Bigger Reactors** 0.5.2, the smallest possible reactor size is **3 × 3 × 3**. With the default config, reactors may be built as large as **128 × 128 × 192**, however this may be changed to an absolute maximum of **192 × 192 × 256**.

## Components

### Required

The following components are the bare minimum required to construct any type of reactor.

* **Reactor Terminals**: are the heart of your reactor.
* **Reactor Casings**: make up the frame and walls of your reactor.
* **Fuel Rods**: are where Fuel and Waste are contained.
* **Control Rods**: are used to maintain control over the reaction.
* **Access Ports**: are used to insert Fuel and extract Waste.

### Type-Specific

Certain components may only be used with a specific type of reactor, and cannot be used together in the same reactor.

The first type of reactor are **Passive Reactors**. These output the energy they generate directly as RF, which may be used by other machines.

* **Power Taps** are where you extract power from a passive reactor.

The second type of reactor are **Active Reactors**. These convert the energy they generate into heat, which is used to heat up fluids.

* **Coolant Ports** are used to insert “cold” fluids (such as water) and extract “hot” fluids (such as steam).
* **Coolant Manifolds** are used to increase the surface area for heat transfer.

### Optional

Some components are entirely optional and are not required to build a functioning reactor. These may, however, allow for automation and remote control of reactors.

* **Redstone Ports** allow for control of various reactor functions via Redstone circuits.
* **Computer Ports** allow for control of various reactor functions via Lua scripting. This requires a computers mod such as CC: Tweaked to be installed.
* **Reactor Glass** functions identically to casings, but may only be used on walls. It allows you to see inside of the reactor.

## Moderators

**Reactor Moderators** (_commonly incorrectly referred to as **Reactor Coolants**_) are materials placed inside of a Reactor during construction. When a reactor is in operation, a moderator may change the way the reactor performs depending its properties.

**Moderators** have four main properties that affect the reactor simulation:

* **Absorption**: The speed at which radiation is absorbed and converted to case heat.
* **Efficiency**: How efficiently absorbed radiation is converted into heat.
* **Moderation**: The effectiveness at which radiation is moderated (“softened”).
* **Conductivity**: How well heat is transferred from the fuel rods to the reactor casing.

In general, higher values are always better (except for absorption, which may be better or worse depending on your reactor design). For a more in-depth explanation on how to use the information here, see the [simulation page](https://biggerseries.net/en/biggerreactors/reactor/simulation).

Something to note is that Modpack authors have the ability to add or modify moderators. For an accurate list of supported blocks/fluids, use [Just Enough Items (JEI)](https://www.curseforge.com/minecraft/mc-mods/jei) by checking the uses for the Reactor Terminal ( **currently broken on multiplayer**).

### Moderator Properties

_The values listed below are accurate for Bigger Reactors 0.5.2, for Minecraft 1.16.5. Also correct for 0.6.x (1.17-1.19)_



<table><thead><tr><th width="290">ID</th><th width="124">Absorption</th><th width="114">Efficiency</th><th width="124">Moderation</th><th width="134">Conductivity</th></tr></thead><tbody><tr><td>astralsorcery:liquid_starlight</td><td>0.85</td><td>0.8</td><td>2.0</td><td>3.0</td></tr><tr><td>biggerreactors:ludicrite_block</td><td>0.6</td><td>0.87</td><td>3</td><td>3</td></tr><tr><td>bloodmagic:life_essence_block</td><td>0.7</td><td>0.55</td><td>1.75</td><td>2.5</td></tr><tr><td>mekanism:ethene</td><td>0.37</td><td>0.65</td><td>1.9</td><td>1.5</td></tr><tr><td>mekanism:hydrofluoric_acid</td><td>0.6</td><td>0.45</td><td>1.4</td><td>2.5</td></tr><tr><td>mekanism:hydrogen</td><td>0.2</td><td>0.3</td><td>1.2</td><td>0.1</td></tr><tr><td>mekanism:hydrogen_chloride</td><td>0.31</td><td>0.65</td><td>1.7</td><td>1</td></tr><tr><td>mekanism:lithium</td><td>0.7</td><td>0.6</td><td>1.04</td><td>0.7</td></tr><tr><td>mekanism:oxygen</td><td>0.01</td><td>0.35</td><td>1.04</td><td>0.1</td></tr><tr><td>mekanism:sodium</td><td>0.23</td><td>0.6</td><td>1.7</td><td>1</td></tr><tr><td>mekanism:steam</td><td>0.33</td><td>0.5</td><td>1.33</td><td>0.5</td></tr><tr><td>mekanismgenerators:deuterium</td><td>0.03</td><td>0.3</td><td>1.07</td><td>0.1</td></tr><tr><td>minecraft:air</td><td>0.1</td><td>0.25</td><td>1.1</td><td>0.05</td></tr><tr><td>minecraft:cave_air</td><td>0.1</td><td>0.25</td><td>1.1</td><td>0.05</td></tr><tr><td>minecraft:glass</td><td>0.2</td><td>0.25</td><td>1.1</td><td>0.3</td></tr><tr><td>minecraft:ice</td><td>0.33</td><td>0.33</td><td>1.15</td><td>0.1</td></tr><tr><td>minecraft:snow_block</td><td>0.15</td><td>0.33</td><td>1.05</td><td>0.05</td></tr><tr><td>minecraft:void_air</td><td>0.1</td><td>0.25</td><td>1.1</td><td>0.05</td></tr><tr><td>minecraft:water</td><td>0.33</td><td>0.5</td><td>1.33</td><td>0.1</td></tr><tr><td>minecraft:lava</td><td>0.33</td><td>0.33</td><td>1.15</td><td>0.7</td></tr><tr><td>forge:storage_blocks/allthemodium</td><td>0.66</td><td>0.9</td><td>3.5</td><td>3.5</td></tr><tr><td>forge:storage_blocks/aluminum</td><td>0.5</td><td>0.78</td><td>1.42</td><td>0.6</td></tr><tr><td>forge:storage_blocks/bronze</td><td>0.51</td><td>0.77</td><td>1.41</td><td>1</td></tr><tr><td>forge:storage_blocks/copper</td><td>0.5</td><td>0.75</td><td>1.4</td><td>1</td></tr><tr><td>forge:storage_blocks/diamond</td><td>0.55</td><td>0.85</td><td>1.5</td><td>3</td></tr><tr><td>forge:storage_blocks/electrum</td><td>0.53</td><td>0.82</td><td>1.47</td><td>2.2</td></tr><tr><td>forge:storage_blocks/emerald</td><td>0.55</td><td>0.85</td><td>1.5</td><td>2.5</td></tr><tr><td>forge:storage_blocks/enderium</td><td>0.53</td><td>0.88</td><td>1.6</td><td>3</td></tr><tr><td>forge:storage_blocks/gold</td><td>0.52</td><td>0.8</td><td>1.45</td><td>2</td></tr><tr><td>forge:storage_blocks/graphite</td><td>0.1</td><td>0.5</td><td>2</td><td>2</td></tr><tr><td>forge:storage_blocks/invar</td><td>0.5</td><td>0.79</td><td>1.43</td><td>0.6</td></tr><tr><td>forge:storage_blocks/iron</td><td>0.5</td><td>0.75</td><td>1.4</td><td>0.6</td></tr><tr><td>forge:storage_blocks/lead</td><td>0.75</td><td>0.75</td><td>1.75</td><td>1.5</td></tr><tr><td>forge:storage_blocks/lumium</td><td>0.75</td><td>0.55</td><td>1.5</td><td>1.8</td></tr><tr><td>forge:storage_blocks/nickel</td><td>0.5</td><td>0.82</td><td>1.46</td><td>0.6</td></tr><tr><td>forge:storage_blocks/osmium</td><td>0.51</td><td>0.77</td><td>1.41</td><td>1</td></tr><tr><td>forge:storage_blocks/platinum</td><td>0.53</td><td>0.86</td><td>1.58</td><td>2.5</td></tr><tr><td>forge:storage_blocks/signalum</td><td>0.63</td><td>0.66</td><td>1.5</td><td>1.8</td></tr><tr><td>forge:storage_blocks/silver</td><td>0.51</td><td>0.79</td><td>1.43</td><td>1.5</td></tr><tr><td>forge:storage_blocks/steel</td><td>0.5</td><td>0.78</td><td>1.42</td><td>0.6</td></tr><tr><td>forge:storage_blocks/tin</td><td>0.3</td><td>0.7</td><td>1.35</td><td>0.75</td></tr><tr><td>forge:storage_blocks/unobtainium</td><td>0.95</td><td>0.82</td><td>2</td><td>5</td></tr><tr><td>forge:storage_blocks/vibranium</td><td>0.15</td><td>0.75</td><td>8</td><td>4</td></tr><tr><td>forge:storage_blocks/zinc</td><td>0.51</td><td>0.77</td><td>1.41</td><td>1</td></tr><tr><td>biggerreactors:liquid_obsidian</td><td>0.3</td><td>0.7</td><td>1.35</td><td>0.75</td></tr><tr><td>allthemodium:molten_allthemodium</td><td>0.66</td><td>0.9</td><td>3.5</td><td>3.5</td></tr><tr><td>allthemodium:molten_vibranium</td><td>0.15</td><td>0.75</td><td>8</td><td>4</td></tr><tr><td>allthemodium:molten_unobtainium</td><td>0.95</td><td>0.82</td><td>2</td><td>5</td></tr><tr><td>allthemodium:vapor_allthemodium</td><td>0.66</td><td>0.9</td><td>3.5</td><td>3.5</td></tr><tr><td>allthemodium:vapor_vibranium</td><td>0.15</td><td>0.75</td><td>8</td><td>4</td></tr><tr><td>allthemodium:vapor_unobtainium</td><td>0.95</td><td>0.82</td><td>2</td><td>5</td></tr><tr><td>forge:superheated_sodium</td><td>0.23</td><td>0.6</td><td>1.7</td><td>1</td></tr><tr><td>forge:redstone</td><td>0.75</td><td>0.55</td><td>1.6</td><td>2.5</td></tr><tr><td>forge:ender</td><td>0.9</td><td>0.75</td><td>2.0</td><td>2</td></tr></tbody></table>
