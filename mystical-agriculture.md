# Mystical Agriculture

## Farm Designs

### AlfredGG’s Farm

{% embed url="https://www.youtube.com/watch?v=iLSlFHweJsI" %}

<details>

<summary>My Watering Can/Scythe isn’t working</summary>

**Mystical Agriculture** doesn’t allow fake players by default. The config can be changed in `config/mysticalagriculture-common.toml` -> `fakePlayerWatering = true`.

</details>

<details>

<summary>My Modular Routers aren’t working</summary>

You will need to add a **Security Upgrade** since you are working in a claimed chunk (even though it’s yours)

</details>

### KJM’s Full-Auto Phytogenic Insolator with AE2

![Full setup using all 32 channels of a dense cable per wall](.gitbook/assets/phytoae2_1.png)

#### Requirements

**Minimum Building Materials**

* These materials set the ground work to build the full thing.
* 3x ME Interface
* 2x ME Storage Bus
* 2x Quartz Fiber or Cable Anchor
* 2x AE2 Crafting Card
* 2x Phytogenic Insolator
* 1x ME Controller
* 1x Pair of Quantum Rings
* 1x Sink/Eternal Water Block
* 1x of **any** colored cable _(Examples are using Magenta cables)_
* 2x of a **different** colored cable _(Examples are using Lime cables)_
* 8x of **another different** colored **Dense** cable _(Examples are using Orange dense cables)_

**All Building Materials**

* 129x ME Interfaces
* 2x ME Storage Bus
* 2x Quartz Fiber or Cable Anchor
* 128x AE2 Crafting Card
* 256x Phytogenic Insolator
* 1x ME Controller
* 1x Pair of Quantum Rings
* 1x Sink/Eternal Water Block
* 1x of **any** colored cable _(Examples are using Magenta cables)_
* 2x of a **different** colored cable _(Examples are using Lime cables)_
* 68x of **another different** colored **Dense** cable _(Examples are using Orange dense cables)_

Each image has a caption that shows when you click on it that you can read if you are stuck.

This farm requires a general understanding of **AE2** and **Thermal Series**

#### The “Brain”

First I’ll show you how to build the “brain” of those whole system. You can place it above everything (like in the image above) or underneath the floor.

{% stepper %}
{% step %}
### Place the Sink, Interface, and Quartz Fibers

Place a **Sink/Eternal Water Block** and an **ME Interface** on the corners of a **Quantum Ring** and then place **2x Quartz Fibers/Cable Anchors** between the Sink and ME Interface and on the center of the Quantum Ring.

![Make sure to put quartz fiber or cable anchors to isolate the Lime cable from your home AE2 system](.gitbook/assets/phytoae2brain_1.png)
{% endstep %}

{% step %}
### Add the colored cables and ME Controller

Then place your **2x colored cables** (Lime cables) on top of them along with an **ME Controller**.

The **1x colored cable** (Magenta cable) should connect the quantum ring and the ME Interface.

* Make sure to link your Quantum Rings.
{% endstep %}

{% step %}
### Add the storage buses

Place **2x ME Storage Bus** on the ME Interface and Sink, facing each other.

![ME Storage Bus on both the Sink and ME Interface](.gitbook/assets/phytoae2brain_2.png)
{% endstep %}

{% step %}
### Set the ME Interface

Have the **ME Interface** stock **Water** and **Phyto-Gro** and set the priority to **-1**.

![ME Interface settings](.gitbook/assets/phytoae2brain_interfacesettings.png)
{% endstep %}

{% step %}
### Set the storage bus on the Sink

For the **ME Storage Bus on the Sink** settings, have the **Input/Output Mode** to **Extract Only** and put **Water** in the filter by dragging it from JEI.

![Storage Bus on sink settings](.gitbook/assets/phytoae2brain_sinkbus.png)
{% endstep %}
{% endstepper %}

#### The Modules

Now we’ll build one of the “modules” that make up the entire thing. Each column of Phyto/Interface pairs is **8 blocks tall** since an AE2 subnet without a controller only has 8 channels. Each wall will use all 32 channels of a dense cable.

{% stepper %}
{% step %}
### Build the module shape

Each module consists of **2 Phytos** next to each other and an **ME Interface** on each side.

![](.gitbook/assets/phytoae2_module.png)

If you build the full size farm, the corners will look like this. One of the Phytos will move 90° to one side depending on which corner it’s on.

![](.gitbook/assets/phytoae2_modulecorner.png)
{% endstep %}

{% step %}
### Set the ME Interface

For the **ME Interface**, put a **Crafting Card** in and set **Water** and **Phyto-Gro** in the filter by dragging it from JEI.

![](.gitbook/assets/phytoae2_cardandfilter.png)
{% endstep %}

{% step %}
### Set the Phytos

For the Phytos it’ll be slightly different depending on which side the ME Interface is on. You will have it **Auto Input/Output** the side touching the interface. The image below is for a phyto with an interface to the left.

![](.gitbook/assets/phytoae2_phytosettings.png)
{% endstep %}

{% step %}
### Add the augments

Each Phyto will have **1x Draconic Integral Component & 3x Twinite Flux Linkages**. This combination provides maximum efficiency, of course you can put the lower tier ones in as you are working up to these.

![](.gitbook/assets/phytoae2_phytoaugs.png)
{% endstep %}
{% endstepper %}

Why not use Shellite instead of Twinite? KJM explains

The stats for Shellite Flux Linkage is 120% & 1.1x. The stats for the Twinite Flux Linkage is 110% & 1.01x. An MA seed uses 20,000FE to complete one growth operation, and Phytos fill at 20FE/t by default. That 20,000 number is multiplied by the process energy statistic. A single Shellite upgrade would modify it to 22,000FE, and Twinite goes to 20,200FE. The second stat modified is energy usage. Shellite increases the per-tick power consumption to 44FE/t, and Twinite increases it to 42FE/t. A recipe runs for 50 seconds by default since 20,000 divided by 20 divided by 20 (the number of ticks per second) is 50. Placing the numbers in for shellite 22,000/44/20 = 25 and for Twinite 20,200/42/20 = 24. Therefore, Twinite at a base level with a single upgrade is 1 second faster than Shellite. This number is further modified by adding multiple linkages and the integral component.

You’ll stack these modules to a **maximum of 8 tall** and arrange them into 4 walls.

Tips

* Use an AE2 **Memory Card** to copy **ME Interface** settings (`Shift + R-Click` to **Copy**, `R-Click` to **Paste**)
* Use **Redprint** to copy **Phytogenic Insolator** settings (`R-Click` to **Copy** and to **Paste**)

#### Connecting and Powering

You’ll put your **Colored Dense Cables** in this arrangement, each dense cable branch connects 4 colums of interfaces. You can use whatever energy pipe you want to power the phytos.

![Full setup using all 32 channels of a dense cable per wall](.gitbook/assets/phytoae2_energy.png)

[Mystical Agriculture | CurseForge](https://legacy.curseforge.com/minecraft/mc-mods/mystical-agriculture)
