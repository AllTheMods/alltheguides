---
title: F.A.Q
description: Frequently Asked Questions
--- 

# F.A.Q

##### This F.A.Q is put into 3 sections. 

- [Technical](#technical)
- [Gameplay](#gameplay)
- [Servers](#servers)

This will attempt to cover all packs.

---
## Technical
#### Table Of Contents -

* [Failed To Authenticate](#failed-to-authenticate).
* [Modpack Crashes (At Beginning)](#modpack-crashes-at-beginning).
* [World Crashing (Before / After)](#world-crashing-before-after).
* [Ticking Entity Or Block](#ticking-entity-or-block).

---

**Context Keywords**

- **Instance**: The specific modpack or profile folder in question.
- **Arguments**: Commands/Flags used with Java to help with performance (Most Garbage Collection).
- **Allocate**: The amount of ram assigned to minecraft. _By default it's always set to 4Gb or lower, and some modpack requires more._

---

### Failed To Authenticate

??? Info

    Authentication errors can be caused by numerous reasons. TL;TD here's some things you can try/check.

    - Restarting Networking (Unplugging router/modem ("Internet Box(es)")).
    - Are you using or have **Hamachi** installed? If installed but not using, this could be a culprit.
    - IPv6 issues. 
        - Setting this Java argument to force IPv4 `-Djava.net.preferIPv4Stack=true`
        - Disabling "Internet Protocol Version 6 (TCP/IPv6)" in/on Adapter Settings in Network and Sharing Center.
    - Flushing DNS > Command Prompt > `ipconfig /flushdns`
    - Firewall / DDoS protection (Modded MC can potentially flood network with packets considering to be an attack and blocking a specific server ip/inbound connections).

### Modpack Crashes (At Beginning)

??? Info

    Crashes can be caused by numerous of reasons, which can be frustrating to figure out exactly why you're crashing.

    - Check within launcher/instance settings there's enough ram allocated. (**8GB** / **8,192MB**). No more than (**12GB** / **12,288MB**).
    - Check you're using the correct (_not latest_) version of **Forge** required for the pack, additionally [Java](java.md)
    - Update GPU drivers, and ensure you're using your **Dedicated GPU**.
        - If **AMD**,
            - Go to [Official AMD Website](https://www.amd.com/en/support) and download / update GPU drivers.
        - If **NVidia**,
            - Go to **NVidia Control Panel**, Update Driver and go to **3D Settings**.
            - Select **Program Settings** tab, and click **Add**
            - **Sort By** by **Recently Used**, and select **Java**. :material-information-outline:{ title="OpenJDK, Adoptium, Amazon Corretto, Microsoft Java, Eclipse Temurin, GraalVM, Adoptium" }
    - Repair Installation, and or delete **Minecraft** / **Forge** `libraries` folder.
        - **CurseForge**: `%USERPROFILE%\curseforge\minecraft\Install`
    - Repair Configs
        - Delete `instance/config` & `instance/kubejs`folders.
        - Download the pack files (not server) from **CurseForge**
        - Inside the archived zip, copy the `overrides/config` and `overrides/kubejs` folder to your `instance` folder.
    - Repair / Re-Install Profile (Pack).
        - Not all launchers have this, therefor you may need to create another instance of the pack.
            **Caution**: If you delete current instance, you may delete your single player worlds! Make sure you back them up.

### World Crashing (Before / After)

??? Info

    Crashing worlds can suck. Some of the most common, if non of the above fixed the issue.
    
    - Corrupted **Configs**
    - Corrupted **Player Data**
    - Corrupted **Chunks**
    - [Ticking Entity Or Block](#ticking-entity-or-block)
    - **Mods** that's being problematic (Bugs, or Additional mods you've installed).

    Some things you can try if,

    - **Delete** `saves?/world/serverconfigs/` folder.
        - **Note**: If a world crash / fail to properly save, `serverconfigs` can potentially get corrupted.
    - Repair Configs
        - **Delete** `instance/config` & `instance/kubejs`folders.
        - Download the **pack files** (_not server_) from **CurseForge**
        - Inside the archived zip, copy the `overrides/config` and `overrides/kubejs` folder to your `instance` folder.
    - Upload the most recent crash report prior to crashing within `instance/crash-reports/` folder to [MC Logs](https://mclo.gs)
        - MCLogs can sometimes point of the issue within the crash report.


### Ticking Entity Or Block

??? Info

    Ticking entities or blocks occurs by what they might've interacted with, loaded / done incorrectly, or perhaps even an un/known discovered bug. 
    
    Lucky there's a trick you _could_ do to possible fix this, if not manually.

    - Locate & Open `saves?/world/serverconfig/forge-server.toml` with any text editor.
        - For **Block Entities**: Set `removeErroringBlockEntities` to `true`.
        - For **Ticking Entities**: Set `removeErroringEntities` to `true`.
        - Load world, save `/save-all` & `/stop`, and set back `false`
            - **Caution**: This should **NOT** be left on for long as it can cause issues removing things if lag is created.

    - Upload the most recent crash report prior to crashing within `instance/crash-reports/` folder to [MC Logs](https://mclo.gs).
        - It can help identify the source of the ticking entity, or at-least what's ticking and from what mod and the position.
        - If you don't have the location of this entity in crash report, or not sure of the exact player position that's near it,
            - Worst cast scenario, removing one of the mods involved in the crash, loading the world once and adding the mod back _sometimes_ fixes the issue.  Make sure you **backup** your world prior.
            - Submit crash report (_MC Logs_) link to the us via GitHub or Discord. 
        - If have the location of this ticking entity, download an **NBT** editor: [NBT Explorer](https://github.com/jaquadro/NBTExplorer) or [NBT Studio](https://github.com/tryashtar/nbt-studio), as it will be handy.
            - **Player**
                - With **NBT** editor of choice, open your `world/playerdata/<player-uuid>.dat` file. You can use [Minecraft UUID](https://mcuuid.net/) to figure out player **UUID**. Open up the player tree and then locate player `X, Y, Z` coordinates.
            - **Coordinates**
                - Use this [Minecraft Coordinate Calculator](https://minecraft.tools/en/coordinate-calculator.php) and input the **Block Position**. You're then given your `X, and Z` **Chunk Section**, along with your **Region** information / file `.mca`.
                - With **NBT** editor, Open your the **Region** `.mca` file in `world/regions`, or `world/entities` if it's mod entity. Look for `Chunk [-,-] @ World (X,Z)` where `World (X, Z)` is the **Chunk Section**.
                    - Note: **Nether** is in **DIM-1** and **End** is in **DIM1** folder. Other dimensions would be in the `dimensions` folder respectively.
                - After chunk is found, open the tree and look for / through entities for the crashing entity.
                    - **Note**: You can also use the **Search** function above and search for the **Value** of the entity name.
                    - **Note #2**: Searching will search within the last location / tree index your mouse clicked.
        - If all still fails, feel free to send us your log or crash report from [MC Logs](https://mclo.gs) to our Github or Discord

---

## Servers
#### Table Of Contents -

---

## Gameplay
#### Table Of Contents -