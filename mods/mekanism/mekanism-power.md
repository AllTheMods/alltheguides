# Mekanism Power

### Power Gen Changes

#### Buffed

| Generator         | Change           | Notes                                                             |
| ----------------- | ---------------- | ----------------------------------------------------------------- |
| **Bio Generator** | ~~280~~ 500 RF/t | Makes it more of an option instead of straight out using **GBG**. |

#### Nerfed

| Generator        | Change              | Notes                                    |
| ---------------- | ------------------- | ---------------------------------------- |
| **GBG Ethylene** | ~~78K~~ \~8.5k RF/t | _Super nerfed_ but promotes good setups. |

Higher burn rate = more melons needed for setup.

Recipe has been made harder for the **GBG**.

***

## AE2 Mekanism Infuser Auto-Crafting

Using **ME Pattern Providers**, we can fully automate the **Metallurgic Infuser** and **Enrichment Chamber**. This setup will only use 2 channels of your main network.

**Materials**

* 1x Metalluric Infuser (higher the level, the better)
* 1x Enrichment Chamber (higher, the better)
* 1x Quartz Fiber
* 8x AE2 Cables
* 2x ME Pattern Provider (Block form)
* 1x ME Interface (Panel form)
* 2x ME Storage Bus
* 8x Blank Patterns

Do you have Refined Obsidian automated already?

You can skip the **Obsidian Dust** filter on the left storage bus and the **Refined Obsidian Dust Pattern** and instead make a processing pattern to turn **Refined Obsidian Ingots** into **Refined Obsidian Dust** and put that in a **Pattern Provider** connected to a **Crusher**.

***

## Building and Configuring

{% stepper %}
{% step %}
#### Put down the **Metallurgic Infuser**

Place an **ME Storage Bus** on both sides of the infuser.
{% endstep %}

{% step %}
#### Place the **ME Pattern Provider**

Place it right behind the infuser and put an **ME Interface** on **top**, then place a **Quartz Fiber** on the side.
{% endstep %}

{% step %}
#### Connect the AE2 devices

Place **7 AE2 cables** (Yellow in the example) connecting _all_ AE2 devices. The orange cable connects to your main AE2 network.

![](../../.gitbook/assets/infuserBuildStep1.png)
{% endstep %}

{% step %}
#### Add the **Enrichment Chamber**

Adjacent to the **Infuser**, place an **Enrichment Chamber** and a **Pattern Provider** behind it and place a cable connecting **both** pattern providers.

If you’re using the same colored cables, place a **Cable Anchor** between them or use a different color.

{% tabs %}
{% tab title="Same Colored Cables" %}
![](../../.gitbook/assets/infuserBuildsStep2.png)
{% endtab %}

{% tab title="Different Colored Cables" %}
![](../../.gitbook/assets/infuserBuildsStep2.1.png)
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
#### Set the machine inputs and outputs

Set the **Infuser** & **Enrichment** inputs/outputs like the images below.

![](../../.gitbook/assets/infuserEnrichIO.png)

The **Infuser** will input items on the left (Red Slot) and Extra Items on the right (Yellow Slot) while the **Enrichment Chamber** will input/output the back (Purple).
{% endstep %}

{% step %}
#### Configure the **ME Storage Buses**

For the **ME Storage Buses** item filters have **Iron**, **Infused Alloy**, **Enriched Alloy**, and **Obsidian Dust** on the _left_ side and **Enriched Redstone**, **Diamond**, and **Obsidian** on the _right_.

![](../../.gitbook/assets/infuserStorageBusConfig.png)
{% endstep %}
{% endstepper %}

***

### Processing Patterns

Now, we’ll encode the **Processing Patterns**. These patterns are made so there will be a _(essentially)_ 0% chance of clogging the Infuser due to leftover materials.

Make sure to set the patterns to **Process** (Furnace icon) instead of **Crafting** (Crafting Table icon).

{% tabs %}
{% tab title="Infuser Patterns" %}
* 8 Iron + 1 Enriched Redstone = 8 Infused Alloy
* 4 Infused Alloy + 1 Enriched Diamond = 4 Enriched Alloy
* 2 Enriched Alloy + 1 Enriched Obsidian = 2 Atomic Alloy
* 1 Obsidian = 4 Obsidian Dust

![](../../.gitbook/assets/infuserPatterns.png)
{% endtab %}

{% tab title="Enrichment Chamber Patterns" %}
* 1 Redstone = 1 Enriched Redstone
* 1 Diamond = 1 Enriched Diamond
* 1 Refined Obsidian Dust = 1 Enriched Obsidian
* 8 Obsidian Dust + 1 Enriched Diamond = 8 Refined Obsidian Dust

![](../../.gitbook/assets/enrichmentPatterns.png)
{% endtab %}
{% endtabs %}

Then you’ll put patterns in each pattern provider as shown below.

![](../../.gitbook/assets/infuserPatternProvider.png)

Make sure to give both machines power and to enabled `Auto-Split`.

***

## Fission Reactor Temp Calculation

**Big shoutout to Kayla for these equations! Go check out her** [**CC Mek SCADA on GitHub!**](https://github.com/MikaylaFischler/cc-mek-scada/wiki)

Use the equation below to estimate how hot your reactor will get at a specific burn rate for either water or sodium coolant. _Remember the reactor starts taking damage at >1200K!_

**Water**: `burn_rate`

\\\* 2 \\\* \[1,000,000 \\\* (`heat_capacity`-1)] + 373.15

**Sodium**: `burn_rate`

\\\* \[1,000,000 \\\* (`heat_capacity`-1)] + 373.15

How do I calculate `heat_capacity`?

`heat_capacity` is joules per kelvin based on the physical size of the reactor, by default thats 1000x the amount of ‘casing’ which includes reactor glass, casing, valves, etc.

\- Kayla

`heat_capacity` = (2 \\\* W2) + \[(H-2) \\\* (W2 -(W-2)2)] \\\* 1000

W and H are the Width and Height of Fission Reactor respectively

[Full Explanation of Kayla’s Calculations](https://github.com/MikaylaFischler/cc-mek-scada/wiki/Reactor-Temperature-Calculation)
