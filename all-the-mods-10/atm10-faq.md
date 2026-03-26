# ATM10 FAQ

**All The Mods 10** Frequently Asked Questions

## Gameplay FAQs

<details>

<summary>There’s a ghost/easter egg that appears every few minutes!</summary>

The ghost is from Corail Tombstone, you can disable by doing `/tbgui` locate the ghost toggle under effect. This toggle will only show if your GUI scale is set to 4.

If you want to prevent the ghost/easter eggs and all other Corail holiday events **permanently**, you can download [BadCorailNoHolidays](https://legacy.curseforge.com/minecraft/mc-mods/badcorailnoholidays), if you want keep some events enabled, it does have a config at `atmInstall/configs/badcorailnoholidays-common.toml`.

</details>

<details>

<summary>How do I change `/home`, `/tpa` etc cooldown?</summary>

To change the behavior of `/home` or to re-enable `/back` and `/rtp`, edit `saves/worldName/serverconfig/ftb-essentials.snbt`. **The world/server has to be stopped for the changes to take effect.**

</details>

<details>

<summary>I can’t complete ‘`questName`’ even though I fufilled the requirements?</summary>

You can enable edit quests in the bottom right of the quest screen (you need OP for this) and then r-click the broken quest and `Complete Instantly` it OR click the quest then r-click the reward and `Reset Progress` if you still want the rewards.

</details>

<details>

<summary>How do I increase claimed/force loaded chunks?</summary>

* Add claimed chunks: `/ftbchunks admin extra_claim_chunks <player> <set/add> <amount>`
* Add force-loaded chunks: `/ftbchunks admin extra_force_load_chunks <player> <add/set> <amount>`

</details>

<details>

<summary>When I mine Allthemodium/Vibranium/Unobtainium it doesn’t drop anything!</summary>

It’s caused by the `Miner's Fervor` enchantment, remove it and try breaking it again.

</details>

## Technical FAQs

<details>

<summary>Why isn’t ‘`insert mod name`’ in ATM10 yet?</summary>

ATM packs does not literally contain “All The Mods”. Our main focus is having mods that’s not: 1) buggy, 2) ruins performance or progression and 3) is updated to 1.21. If a mod supports Minecraft version **1.21**, and **Neo Forge**, you may make a [suggestion](https://github.com/AllTheMods/ATM-10/issues/2).

</details>

<details>

<summary>I found a bug/dupe in the pack. How can I report it?</summary>

To report bugs, dupes or similar, head over to the [ATM10 GitHub](https://github.com/AllTheMods/ATM-10/issues) and open a new issue describing the occurrence.

</details>

<details>

<summary>My screen is shaking like im getting hurt and I can’t do anything!</summary>

Backup your world, then download [NBT Explorer](https://github.com/jaquadro/NBTExplorer) from GitHub.

{% hint style="warning" %}
Make sure you shutdown your world/server before attempting this!
{% endhint %}

Go to AlltheMods9ATM9\saves\theNameOfYourWorld and open level.dat with NBT Explorer.Go to Date -> Player and set AbsorptionAmount to 1.Scroll down and set Health to 1.Save the file and start your worldGo to world/playerdata and find the affected player’s UUID playerUUID.dat file and open it with NBT Explorer.Go to Date -> Player and set AbsorptionAmount to 1.Scroll down and set Health to 1.Save the file and start your server.

</details>

<details>

<summary>What are the recommended Java arguments for this pack?</summary>

* **Client arguments**: send `?args21` in the **#bot-spam** channel in our [Discord](https://discord.com/invite/allthemods).
* **Server arguments**: send `?svargs21` in the **#bot-spam** channel in our [Discord](https://discord.com/invite/allthemods).
* Check out the [Java](/broken/pages/df9899090c88cd329688907151c4d8149a707c2b#java-arguments) section

</details>

<details>

<summary>Why does my game crash while launching?</summary>

Lack of RAM most likely. Send `?allocate` in the **#bot-spam** channel in our [Discord](https://discord.com/invite/allthemods) to learn how to allocate more RAM. If that’s not the problem, head to **#atm10-techsupport** and send `?logs` to see how to upload your crash/latest log.

</details>

<details>

<summary>I crashed and got `Error code 1`, please help</summary>

`Exit code 1` is a generic error from Minecraft. It is no different than “game didn’t load, no longer attempting to load. Please refer to the output error log created by your launcher” if you are unsure… please feel free to ask for further instructions on how to locate, post, and get help for your specific error so that we may further assist you in our [Discord](https://discord.com/invite/allthemods). Try running `?logs` instead.

</details>
